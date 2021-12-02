# Xournal++

[![Build Status](https://dev.azure.com/xournalpp/xournalpp/_apis/build/status/CI?branchName=master)](https://dev.azure.com/xournalpp/xournalpp/_build/latest?definitionId=1&branchName=master)
[![Join the chat at https://gitter.im/xournalpp/xournalpp](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/xournalpp/xournalpp?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

<table border="0px" ><tr><td width = 600px>

<img src="readme/main.png" width=550px% title="Xournal++ Screenshot on Linux"/>

</td><td>

## Alerta! - Precisamos de tradutores!

Recentemente, revisitamos a caixa de diálogo de configurações para melhorar a sensação e a usabilidade.
Ao fazer isso, também adicionamos descrições melhores, para as quais exigimos
novas traduções.

Traduções parciais, que precisam ser atualizadas:

- Tcheca
- Polonês
- Chinês

Traduções completas para todos os idiomas não mencionados anteriormente **exceto**:

- Inglês
- Alemâo
- Italiano

Se você quiser nos ajudar a melhorar a localização do Xournal ++, dê uma olhada em [nosso projeto Crowdin](https://crowdin.com/project/xournalpp). Se você estiver interessado em traduzir um novo idioma, entre em contato conosco no [Gitter](https://gitter.im/xournalpp/xournalpp) ou crie um novo fascículo e nós desbloquearemos o idioma no Crowdin.

**Obrigado desde já!**

</td></tr></table>

## Recursos

Xournal++ é um software para tomar notas escrito em C ++ com o objetivo de flexibilidade, funcionalidade e velocidade.
O reconhecedor de traços e outras partes são baseados no código Xournal, que você pode encontrar em [sourceforge](http://sourceforge.net/projects/xournal/)

Recursos do Xournal++:

- Suporta estiletes sensíveis à pressão e mesas de caneta digital (por exemplo, tablets Wacom, Huion, XP Pen, etc.)
- Planos de fundo de papel para anotações, rascunho ou quadro branco
- Faça anotações sobre PDFs
- Exporte para uma variedade de formatos, incluindo SVG, PNG e PDF, tanto da GUI quanto da linha de comando
- Diferentes ferramentas de desenho (por exemplo, caneta, marca-texto) e estilos de traçado (por exemplo, sólido, pontilhado)
- Desenho de forma (linha, seta, círculo, retângulo, spline)
- Funcionalidade de forma de preenchimento
- redimensionamento e rotação da forma
- Rotação e ajuste de grade para alinhamento preciso de objetos
- Estabilização de entrada para escrita / desenho mais suave
- Ferramenta de texto para adicionar texto em diferentes fontes, cores e tamanhos
- Suporte aprimorado para inserção de imagem
- Borracha com múltiplas configurações
- Suporte a LaTeX (requer uma instalação LaTeX funcional) com modelo personalizável
- Barra lateral com visualizações de página com classificação de página avançada, marcadores e camadas de PDF (podem ser ocultados / editados individualmente)
- Permite mapear diferentes ferramentas / cores, etc. para botões da caneta / mouse
- Barra de ferramentas personalizável com várias configurações, por exemplo para otimizar a barra de ferramentas para retrato / paisagem
- Definições de modelo de página
- Relatórios de bugs, salvamento automático e ferramentas de backup automático
- Gravação e reprodução de áudio junto com notas manuscritas
- Suporte multilíngue (mais de 20 idiomas suportados)
- Plugins usando script Lua

## Aplicativo mobile & web

Desde meados de 2020, existe um aplicativo móvel escrito pelo Flutter para ** Android **, ** Chrome OS ** e ** iOS ** (em breve), bem como um ** aplicativo web ** disponível. Mesmo que não seja perfeitamente estável e nem todos os recursos do Xournal ++ sejam totalmente suportados, você pode verificar e abrir seus notebooks Xournal ++ em seus dispositivos móveis. Você pode entrar em contato em seu [repositório no GitLab](https://gitlab.com/TheOneWithTheBraid/xournalpp_mobile).

[Baixe no Google Play](https://play.google.com/store/apps/details?id=online.xournal.mobile)

A versão web é disponibilizada em [xournal.online](https://xournal.online).

_Por que o aplicativo iOS ainda não foi publicado?_

De acordo com as diretrizes da Apple App Store, é proibido publicar aplicativos instáveis ou beta. Portanto, esperamos até que o Xournal ++ Mobile funcione de maneira mais estável e ofereça compatibilidade de recursos mais completa com o Xournal ++.

<table>
<tr>
<td>

## Linux

<img src="readme/main.png" width=100% title="Xournal++ Screenshot on Linux"/>

</td><td>

## Windows 10

<img src="readme/main-win.png" width=100% title="Xournal++ Screenshot on Win10"/>

</td></tr><tr><td>

## macOS Catalina

<img src="readme/main-mac.png" width=100% title="Xournal++ Screenshot on macOS"/>

</td><td>

## Xournal++ Mobile

<img src="https://gitlab.com/TheOneWithTheBraid/xournalpp_mobile/-/raw/master/fastlane/metadata/android/en_US/images/tenInchScreenshots/03.png" width=100% title="Xournal++ Mobile Screenshot on Chromium OS"/>

</td></tr><tr><td>

## Barra de Ferramentas / Fundo da Página / Camada

Plano de fundo de várias páginas, facilmente selecionável na barra de ferramentas
<img src="readme/background.png" width=100% title="Xournal++ Screenshot"/>

</td><td>

## Barra lateral da camada e seleção de camada avançada.

<img src="readme/layer.png" width=100% title="Xournal++ Screenshot"/>

</td></tr><tr><td>

## Barra de ferramentas predefinida e totalmente personalizável.

<img src="readme/toolbar.png" width=100% title="Xournal++ Screenshot"/>

</td></tr></table>

## Manual do usuário e FAQ

Para uso geral, consulte o [Manual de Usuário](https://github.com/xournalpp/xournalpp/wiki/User-Manual). Respostas para
algumas perguntas comuns podem ser encontradas no
[FAQ](https://github.com/xournalpp/xournalpp/wiki/Frequently-Asked-Questions-&-Problem-Solving).

## Recursos experimentais:

Às vezes, é adicionado um recurso que pode não ser sólido como uma rocha ou os desenvolvedores não têm certeza se é útil.
Experimente e dê-nos algum feedback.

Aqui estão alguns em desenvolvimento com os quais você pode jogar agora.

- <img src="readme/floatingtoolboxmbmenu.png"  title="Xournal++ Screenshot"/> Atribua um botão do mouse ou botão da caneta para abrir uma caixa de ferramentas de barras de ferramentas logo abaixo do cursor. Você também pode modificar o que está na caixa de ferramentas através do usual Exibir-> Barras de Ferramentas-> Personalizar, embora **não apareça a menos que você tenha atribuído um botão nas preferências: mouse ou caneta** (ou selecionado uma configuração de barra de ferramentas que usa isto).

 - Este é um recurso experimental porque nem tudo que você pode colocar na caixa de ferramentas se comporta. Portanto, esteja atento.

    <img src="readme/floatingtoolbox.png" width=25% />

* Fique atento a outros recursos experimentais nas preferências, conforme visto aqui:

   DrawingTools: Ao desenhar uma caixa, círculo, etc., simula os modificadores ctrl ou shift pela direção inicial em que você move o mouse.

   Ação no toque da ferramenta: Permitir um breve toque na tela para abrir a caixa de ferramentas flutuante e / ou selecionar um objeto. Pode funcionar apenas com caneta e marcador.

   <img src="readme/moreexperimentals.png" width=50% />

## Instalação

Os lançamentos oficiais do Xournal ++ podem ser encontrados nas
[Atualizações](https://github.com/xournalpp/xournalpp/releases). Nós provemos
binários para Debian (Buster), Ubuntu (16.04), MacOS (10.15 e mais recente) e
Janelas. Para outras distribuições Linux (ou mais antigas / mais recentes), também fornecemos um
AppImage que é binário compatível com qualquer distribuição lançada em torno de ou
após o Ubuntu 16.04. Para instalar o Xournal ++ Mobile em dispositivos portáteis, veja [Intrução para Xournal++ Mobile](https://gitlab.com/TheOneWithTheBraid/xournalpp_mobile#try-it-out)

**Uma observação para usuários do Ubuntu / Debian**: os binários oficiais que fornecemos são
compatível apenas com a _versão específica do Debian ou Ubuntu_ indicada pelo
nome do arquivo. Por exemplo, se você estiver no Ubuntu 20.04, o binário cujo nome
contém `Ubuntu-bionic` é _somente_ compatível com Ubuntu 18.04. Se o seu sistema
não é uma das versões específicas do Debian ou Ubuntu que são suportadas pelo
binários oficiais, recomendamos que você use o PPA (somente Ubuntu), o Flatpak ou o
AppImage.

Também existe uma _unstable_, [automated nightly
release](https://github.com/xournalpp/xournalpp/releases/tag/nightly) onde
inclui os recursos e correções de bugs mais recentes.

Com a ajuda da comunidade, o Xournal ++ também está disponível nos repositórios oficiais
de algumas distribuições e plataformas Linux populares.

### Debian

Aqui estão as [Atualizações estáveis](https://github.com/xournalpp/xournalpp/releases) e
_unstable_ [automated nightly releases](https://github.com/xournalpp/xournalpp/releases/tag/nightly)
para Debian.

### Ubuntu e derivados

#### Stable PPA
A última versão estável está disponível através do seguinte [_unofficial_ PPA](https://github.com/xournalpp/xournalpp/issues/1013#issuecomment-692656810):

```bash
sudo add-apt-repository ppa:apandada1/xournalpp-stable
sudo apt update
sudo apt install xournalpp
```

#### Unstable PPA
Um lançamento noturno _unstable_ está disponível para distribuições baseadas no Ubuntu por meio do seguinte PPA:

```bash
sudo add-apt-repository ppa:andreasbutti/xournalpp-master
sudo apt update
sudo apt install xournalpp
```

Este PPA é fornecido pela equipe do Xournal ++. Embora tenha os recursos mais recentes e
correções de bugs, ele também não foi testado completamente e pode falhar periodicamente (nós
tente o nosso melhor para não quebrar as coisas).

### Fedora

A [released version of
xournalpp](https://src.fedoraproject.org/rpms/xournalpp) está disponível em
[main repository](https://bodhi.fedoraproject.org/updates/?packages=xournalpp)
via aplicação de software do seguinte comando:

```bash
sudo dnf install xournalpp
```

or

```bash
pkcon install xournalpp
```

Os pacotes de última geração sincronizados com xournalpp git master diariamente estão disponíveis em [COPR luya/xournalpp](https://copr.fedorainfracloud.org/coprs/luya/xournalpp/).
[![Copr build status](https://copr.fedorainfracloud.org/coprs/luya/xournalpp/package/xournalpp/status_image/last_build.png)](https://copr.fedorainfracloud.org/coprs/luya/xournalpp/package/xournalpp/)

### openSUSE

No openSUSE Tumbleweed, a versão lançada do Xournal ++ está disponível no
repositório principal:

```bash
sudo zypper in xournalpp
```

Para o openSUSE Leap 15.0 e anterior, use o link de instalação de
[X11:Utilities](https://software.opensuse.org//download.html?project=X11%3AUtilities&package=xournalpp).

Para todas as versões do openSUSE, pacotes de última geração sincronizados com xournalpp git
master em uma base semanal estão disponíveis em
[home:badshah400:Staging](https://software.opensuse.org//download.html?project=home%3Abadshah400%3AStaging&package=xournalpp).

### Arch Linux

A última versão estável está disponível [in the [community]
repository](https://www.archlinux.org/packages/community/x86_64/xournalpp/).

Para construir você mesmo o estado mais recente do branch master, use [this AUR
package](https://aur.archlinux.org/packages/xournalpp-git/).

### Solus

A última versão estável está disponível no repositório principal:

```bash
sudo eopkg it xournalpp
```

### Flatpak

A equipe do Xournal ++ suporta oficialmente uma [Versão FlatHub](https://flathub.org/apps/details/com.github.xournalpp.xournalpp), que
pode ser instalado com

```bash
flatpak install flathub com.github.xournalpp.xournalpp
```

Observe que para o Xournal ++ funcionar corretamente, você deve ter pelo menos um tema GTK
e um tema de ícone instalado no Flatpak. Para habilitar o suporte a LaTeX, você também
precisa instalar a extensão TeX Live:

```bash
flatpak install flathub org.freedesktop.Sdk.Extension.texlive
```

O manifesto Flatpak pode ser encontrado no pacote [Xournal ++ Flatpak
repositório] (https://github.com/flathub/com.github.xournalpp.xournalpp), e todos
Problemas de empacotamento relacionados ao Flatpak devem ser relatados lá.

### Android and Chrome OS

O Android é compatível com o Xournal ++ Mobile. Ele pode ser baixado em [Tags page](https://gitlab.com/TheOneWithTheBraid/xournalpp_mobile/-/tags) ou [from Google Play](https://play.google.com/store/apps/details?id=online.xournal.mobile).

### iOS

Infelizmente, o aplicativo iOS ainda não foi publicado na Apple App Store. Veja [here](#mobile--web-app) para saber por quê. De qualquer forma, em [Building section](#building) você pode aprender como construir uma prévia.

### Windows

Os lançamentos oficiais do Windows são fornecidos em [Releases
page](https://github.com/xournalpp/xournalpp/releases).

**Notas:**

- Atualmente, apenas drivers WinTab são suportados. Isso é devido a uma limitação com
  a biblioteca subjacente que usamos, GTK.
- Existe um bug GTK que impede que a entrada da caneta funcione corretamente. Por favor comece
  Xournal ++, toque com a caneta, saia do Xournal ++ e comece novamente. Então caneta
  entrada estará funcionando, até que você reinicie o Windows. Ver
   [#659](https://github.com/xournalpp/xournalpp/issues/659).

### Mac OS X

As versões do Mac OS X são fornecidas em [Releases
page](https://github.com/xournalpp/xournalpp/releases).

**Notas:**

- Houve problemas de compatibilidade com o Mac OS X Catalina em relação a ambos
  permissões de arquivo e suporte para stylus
  ([#1772](https://github.com/xournalpp/xournalpp/issues/1772) e
  [#1757](https://github.com/xournalpp/xournalpp/issues/1757)). Infelizmente,
  não temos recursos para apoiar adequadamente Catalina neste momento. Ajuda
  seria apreciado!
- Xournal ++ será entregue com um GTK corrigido. Caso contrário, a sensibilidade à pressão não funcionará no Mac
  [#569](https://github.com/xournalpp/xournalpp/issues/569).

## Construindo

[Linux Build](readme/LinuxBuild.md)

[Mac Build](readme/MacBuild.md)

[Windows Build](readme/WindowsBuild.md)

[Android Build](https://gitlab.com/TheOneWithTheBraid/xournalpp_mobile#getting-started)

[iOS Build](https://gitlab.com/TheOneWithTheBraid/xournalpp_mobile#getting-started)

## Formato de arquivo

O formato de arquivo _.xopp é um XML compactado em .gz. Os PDFs não são incorporados ao arquivo, portanto, se o PDF for excluído, o fundo será perdido. _.xopp é basicamente o mesmo formato de arquivo que _.xoj, que é usado pelo Xournal. Portanto, o Xournal ++ é capaz de ler arquivos _.xoj e também exportar para _.xoj. Assim que as notas são exportadas para um arquivo _.xoj, todas as extensões específicas do Xournal ++, como tipos de fundo adicionais, são perdidas.

\*. xopp pode, teoricamente, ser lido pelo Xournal, desde que você não use nenhum recurso novo. O Xournal não abre arquivos que contêm novos atributos ou valores desconhecidos, então o Xournal ++ adicionará a extensão .xopp a todos os arquivos salvos para indicar a presença potencial de recursos exclusivos do Xournal ++.

Todos os novos arquivos serão salvos como _.xopp. Se um arquivo _.xoj criado pelo Xournal for aberto, a caixa de diálogo Salvar como será exibida ao salvar. Se o arquivo \ *. Xoj foi criado pelo Xournal ++, o arquivo será sobrescrito ao salvar e a extensão do arquivo não será alterada.

**No momento, estamos introduzindo um novo formato de arquivo que pode armazenar com eficiência arquivos PDF anexados e outros anexos internamente. Ainda permitiremos anexos vinculados a arquivos externos. Consulte [#937](https://github.com/xournalpp/xournalpp/issues/937) para mais detalhes.**

## Desenvolvimento

Para desenvolver novos recursos, crie um problema ou comente sobre um problema existente para que outras pessoas saibam o que você está fazendo.
Para o desenvolvimento, crie um fork e use o master como base. Crie uma solicitação Pull para cada correção.
Não crie grandes solicitações de pull, contanto que você não quebre nada, os recursos também podem ser
fundidos, mesmo que não estejam 100% concluídos.

Veja [GitHub:xournalpp](http://github.com/xournalpp/xournalpp) para o desenvolvimento atual. Você também pode entrar
nosso canal Gitter através do crachá na parte superior.

Também dê uma olhada em [Coding Conventions](https://github.com/xournalpp/xournalpp/wiki/Coding-conventions)

## Documentação

A documentação do código é gerada usando Doxygen.

Para gerar a documentação por conta própria, primeiro instale o Doxygen e o graphviz, ou seja,

```bash
sudo apt install doxygen
sudo apt install graphviz
```

no Debian ou Ubuntu. Finalmente, digite `doxygen` no diretório raiz do repositório.
A documentação pode ser encontrada em `doc / html` e` doc / latex`. Convenientemente exiba o
documentação com `python3 -m http.server 8000` e visite o URL mostrado para ver o
documentação.
