# Construção do Xournal++ para Linux

## Instalar dependências

O Xournal++ é programado com c++17 e precisa do cabeçalho <optional> e de uma biblioteca de sistema de arquivos, assim como o STL ou a implementação boost.
Portanto, é necessário instalar um compilador que implementa esses recursos.
Recomendamos g++-8 ou clang-9 ou superior.

Crie pull requests (ou file issues) se tiver dependências mais precisas.

Lua é necessária para os plug-ins; se estiver faltando, os plug-ins serão desabilitados.

### Gerador CMake

As instruções de instalação não assumem nenhuma ferramenta de construção específica (além do CMake),
mas eles exigem make, ninja ou outro gerador CMake compatível. É necessário
que tal ferramenta seja instalada para construir o xournalpp.

A versão mínima exigida do CMake é 3.10, mas recomendamos usar>=3.15.

### Comandos específicos de distribuição

#### Para Ubuntu ou Debian:
````bash
sudo apt-get install cmake libgtk-3-dev libpoppler-glib-dev portaudio19-dev libsndfile-dev \
libcppunit-dev dvipng texlive libxml2-dev liblua5.3-dev libzip-dev librsvg2-dev gettext lua-lgi
````

## Compilação

As etapas básicas para compilar o Xournal++ são:

```bash
git clone http://github.com/xournalpp/xournalpp.git
cd xournalpp
mkdir build
cd build
cmake ..
cmake --build .
# Para uma construção mais rápida, defina a flag -DCMAKE_BUILD_TYPE=RelWithDebInfo
```

Use `cmake-gui ..` para configurar graficamente a compilação.

Com Cairo 1.16. Marcadores de PDF serão possíveis, mas esta versão ainda não está
disponível, portanto, o Cairo PDF Export é sem marcadores de PDF.

O executável binário será colocado no subdiretório `build/src/`.

## Empacotamento e Instalação

### Criação de pacotes para gerenciadores de pacotes

Certifique-se de que o destino `translations` tenha sido construído antes
tentando gerar qualquer pacote.
```bash
cmake --build . --target translations
```

Após a compilação, selecione quais pacotes você deseja gerar (veja o respectivo
seções abaixo) e, em seguida, execute o destino `package`. Os pacotes gerados irão
estar localizado em `build/packages`. Por exemplo:

```bash
cmake .. -DCPACK_GENERATOR="TGZ;DEB"  # Gerar pacotes .tar.gz and .deb 
cmake --build . --target package
```

Por padrão, um pacote `.tar.gz` independente será gerado. Por
plataformas de empacotamento agnósticas de distro, como AppImages e Flatpaks, consulte o
seções relevantes abaixo.

#### Pacotes .deb

```bash
cmake .. -DCPACK_GENERATOR="DEB" ..
cmake --build . --target package
```

#### Pacotes .rpm

TODO

#### AppImage

A maneira mais rápida de gerar um AppImage é primeiro gerar o arquivo `.tar.gz`
pacote e, em seguida, use-o com o `azure-pipelines/util/build_appimage.sh`
roteiro.

```bash
cmake .. -DCPACK_GENERATOR="TGZ"
cmake --build . --target package
../azure-pipelines/util/build_appimage.sh
```

O script `build_appimage.sh` baixará automaticamente o LinuxDeploy, copie o
arquivos `.tar.gz` e bibliotecas e recursos necessários em um `appimage_staging`
diretório e execute LinuxDeploy no diretório de aplicativo preparado.

Por padrão, o script `build_appimage.sh` irá copiar o tema Adwaita GTK e
o tema do ícone Adwaita no AppImage.

#### Flatpak

O manifesto Flatpak para Xournal++ está localizado em
https://github.com/flathub/com.github.xournalpp.xournalpp, que deve ser
clonado em um diretório separado antes de construir.

```bash
git clone https://github.com/flathub/com.github.xournalpp.xournalpp xournalpp-flatpak
```

Por padrão, o manifesto Flatpak irá construir a última versão estável do
Xournal++. Você pode alterar a versão construída para um commit específico editando o
confirme as informações do manifesto para o commit desejado (também especifique as tags se
construir uma versão estável):

```diff
   - name: xournalpp
     buildsystem: cmake-ninja
     sources:
       - type: git
         url: https://github.com/xournalpp/xournalpp
-        commit: 14e9012b94e005112387dbb7d2ed59274d542885
-        tag: 1.0.10
+        commit: a911a3911df7c588c23997a29ad6a2e8d48b4aea
+        tag: 1.0.15
```

Você também pode construir seu clone local do Xournal++ alterando o tipo de fonte para
`dir` e especificando o caminho para o clone.

### Instalação por fonte

__Desencorajamos totalmente a instalação por fonte__, pois pode levar a problemas quando
atualizar para versões mais recentes posteriormente. Por favor, pense em criar um pacote nativo,
 um AppImage ou Flatpak em seu lugar. As instruções estão acima.

Se você não quiser fazer um pacote, você pode instalar o Xournal++ em seu usuário
pasta (ou qualquer outra pasta) especificando `CMAKE_INSTALL_PREFIX`:

```bash
cmake .. -DCMAKE_INSTALL_PREFIX=$HOME/.local
cmake --build . --target install
./cmake/postinst configure
```

Se você deseja instalar o Xournal++ em todo o sistema diretamente do diretório de compilação, execute

```bash
cmake .. -DCMAKE_INSTALL_PREFIX=/usr
sudo cmake --build . --target install
./cmake/postinst configure
```
