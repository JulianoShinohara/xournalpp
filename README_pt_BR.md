Xournal++

Xournal ++ é um software para tomar notas escrito em C ++ com o objetivo de flexibilidade, funcionalidade e velocidade. O reconhecedor de traços e outras partes são baseados no código Xournal.

    Recursos do Xournal++

• Suporta estiletes sensíveis à pressão e mesas de caneta digital (por exemplo, tablets Wacom, Huion, XP Pen, etc.)
• Planos de fundo de papel para anotações, rascunho ou quadro branco
• Faça anotações sobre PDFs
• Exporte para uma variedade de formatos, incluindo SVG, PNG e PDF, tanto da GUI quanto da linha de comando
• Diferentes ferramentas de desenho (por exemplo, caneta, marca-texto) e estilos de traçado (por exemplo, sólido, pontilhado)
• Desenho de forma (linha, seta, círculo, retângulo, spline)
• Funcionalidade de forma de preenchimento
• Redimensionar e rotação da forma
• Rotação e ajuste de grade para alinhamento preciso de objetos
• Estabilização de entrada para escrita / desenho mais suave
• Ferramenta de texto para adicionar texto em diferentes fontes, cores e tamanhos
• Suporte aprimorado para inserção de imagem
• Borracha com múltiplas configurações
• Suporte a LaTeX (requer uma instalação funcional de LaTeX) com modelo personalizável
• Barra lateral com visualizações de página com classificação avançada de páginas, marcadores e camadas de PDF (podem ser ocultados / editados individualmente)
• Permite mapear diferentes ferramentas / cores, etc. para botões da caneta / mouse
• Barra de ferramentas personalizável com várias configurações, por exemplo, para otimizar a barra de ferramentas para retrato / paisagem
• Definições de modelo de página
• Relatórios de bugs, salvamento automático e ferramentas de backup automático
• Gravação e reprodução de áudio junto com notas manuscritas
• Suporte multilíngue (mais de 20 idiomas suportados)
• Plugins usando script Lua

    Formato do arquivo

    O formato de arquivo _.xopp é um XML compactado em .gz. Os PDFs não são incorporados ao arquivo, portanto, se o PDF for excluído, o fundo será perdido. _.xopp é basicamente o mesmo formato de arquivo que _.xoj, que é usado pelo Xournal. Portanto, o Xournal ++ é capaz de ler arquivos _.xoj e também exportar para _.xoj. Assim que as notas são exportadas para um arquivo _.xoj, todas as extensões específicas do Xournal ++, como tipos de fundo adicionais, são perdidas.

**.xopp pode teoricamente ser lido pelo Xournal, desde que você não use nenhum recurso novo. O Xournal não abre arquivos que contêm novos atributos ou valores desconhecidos, então o Xournal ++ adicionará a extensão .xopp a todos os arquivos salvos para indicar a presença potencial de recursos exclusivos do Xournal ++.

    Todos os novos arquivos serão salvos como _.xopp. Se um arquivo _.xoj criado pelo Xournal for aberto, a caixa de diálogo Salvar como será exibida ao salvar. Se o arquivo * .xoj foi criado pelo Xournal ++, o arquivo será sobrescrito ao salvar e a extensão do arquivo não será alterada.

    Desenvolvimento

    Para desenvolver novos recursos, crie um problema ou comente sobre um problema existente para que outras pessoas saibam o que você está fazendo. Para o desenvolvimento, crie um fork e use o master como base. Crie uma solicitação Pull para cada correção. Não crie grandes solicitações de pull, desde que você não quebre nada, os recursos também podem ser mesclados, mesmo que não estejam 100% concluídos.
    


