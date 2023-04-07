#Sintaxe básica de gravação e formatação no GitHub

Títulos
Para criar um título, adicione de um a seis símbolos # antes do texto do título. O número de # que você usará para determinar o tamanho do título.

# The largest heading
## The second largest heading
###### The smallest heading
Títulos H1, H2 e H6 renderizados

Ao usar dois ou mais cabeçalhos, o GitHub gera automaticamente uma tabela de conteúdo que você pode acessar clicando em  dentro do cabeçalho do arquivo. Cada título do cabeçalho está listado na tabela de conteúdo e você pode clicar em um título para acessar a seção selecionada.

Captura de tela que destaca o ícone da tabela de conteúdo

Estilo do texto
Você pode indicar ênfase com texto em negrito, itálico, tachado, subscrito ou sobrescrito em campos de comentários e arquivos .md.

Estilo	Sintaxe	Atalho do teclado	Exemplo	Saída
Negrito	** ** ou __ __	Comando+B (Mac) ou CTRL+B (Windows/Linux)	**This is bold text**	Este texto está em negrito
Itálico	* * ou _ _     	Comando+I (Mac) ou CTRL+I (Windows/Linux)	*This text is italicized*	Este texto está em itálico
Tachado	~~ ~~		~~This was mistaken text~~	Este texto contém um erro
Negrito e itálico aninhado	** ** e _ _		**This text is _extremely_ important**	Este texto é extremamente importante
Todo em negrito e itálico	*** ***		***All this text is important***	Todo este texto é importante
Subscrito	<sub> </sub>		<sub>This is a subscript text</sub>	Este é um texto subscrito
Sobrescrito	<sup> </sup>		<sup>This is a superscript text</sup>	Este é um texto sobrescrito
Texto de referência
Você pode citar um texto com >.

Text that is not a quote

> Text that is a quote
Texto citado renderizado

Dica: ao ver uma conversa, você pode citar automaticamente o texto em um comentário realçando o texto e digitando R. Cite um comentário inteiro clicando em  e em Resposta de citação. Para obter mais informações sobre atalhos de teclado, confira "Sobre atalhos do teclado".

Citar código
Você pode chamar código ou um comando em uma frase com aspas simples. O texto entre as aspas não será formatado. Você também pode pressionar o atalho de teclado Comando+E (Mac) ou Ctrl+E (Windows/Linux) para inserir os acentos graves para um bloco de código dentro de uma linha de Markdown.

Use `git status` to list all new or modified files that haven't yet been committed.
Bloco de código inline renderizado

Para formatar código ou texto no próprio bloco distinto, use aspas triplas.

Some basic Git commands are:
```
git status
git add
git commit
```
Bloco de código renderizado

Para obter mais informações, confira "Criar e realçar blocos de código".

Se você estiver editando tabelas e snippets de código com frequência, poderá se beneficiar da habilitação de uma fonte de largura fixa em todos os campos de comentário no GitHub. Para obter mais informações, confira "Sobre gravação e formatação no GitHub".

Modelos de cores com suporte
Em problemas, solicitações de pull e discussões, você pode chamar cores dentro de uma frase usando aspas invertidas. Um modelo de cor com suporte em aspas invertidas exibirá uma visualização da cor.

The background color should be `#ffffff` for light mode and `#0d1117` for dark mode.
Modelo de cor com suporte renderizado.

Veja abaixo os modelos de cores com suporte no momento.

Cor	Sintaxe	Exemplo	Saída
HEX	`#RRGGBB`	`#0969DA`	Modelo de cor com suporte renderizado no formato HEX.
RGB	`rgb(R,G,B)`	`rgb(9, 105, 218)`	Modelo de cor com suporte renderizado no formato RGB.
HSL	`hsl(H,S,L)`	`hsl(212, 92%, 45%)`	Modelo de cor com suporte renderizado no formato HSL.
Observações:

Um modelo de cor com suporte não pode ter espaços à esquerda ou à direita dentro das aspas invertidas.
A visualização da cor só tem suporte em problemas, solicitações de pull e discussões.
Links
Você pode criar um link embutido colocando o texto do link entre colchetes [ ] e colocando a URL entre parênteses ( ). Também é possível usar o atalho de teclado Command+K para criar um link. Quando você tiver o texto selecionado, poderá colar uma URL da área de transferência para criar automaticamente um link por meio da seleção.

Você também pode criar um hiperlink Markdown realçando o texto e usando o atalho de teclado Command+V. Se você quiser substituir o texto pelo link, use o atalho de teclado Command+Shift+V.

This site was built using [GitHub Pages](https://pages.github.com/).

Link renderizado

Dica: o GitHub cria links automaticamente quando URLs válidas são escritas em um comentário. Para obter mais informações, confira "URLs e referências autovinculadas".

Links de seção
Você pode vincular diretamente a uma seção de um arquivo interpretado, passando o mouse sobre o título da seção para expor o link:

Link da seção no arquivo README para o repositório github/scientist

Links relativos
É possível definir links relativos e caminhos de imagens em seus arquivos representados para ajudar os leitores a acessar outros arquivos no repositório.

Um link relativo é um link que é relativo ao arquivo atual. Por exemplo, se você tiver um arquivo LEIAME na raiz do repositório e tiver outro arquivo em docs/CONTRIBUTING.md, o link relativo para CONTRIBUTING.md no LEIAME poderá ter esta aparência:

[Contribution guidelines for this project](docs/CONTRIBUTING.md)
GitHub transformará automaticamente o seu link relativo ou caminho da imagem baseado em qualquer branch em que você estiver no momento para que o link ou caminho sempre funcione. O caminho do link será relativo ao arquivo atual. Links que começam com / serão relativos à raiz do repositório. Você pode usar todos os operandos de link relativos, como ./ e ../.

Os links relativos são mais fáceis para usuários que clonam o seu repositório. Os links absolutos podem não funcionar em clones do seu repositório - recomendamos usar links relativos para referir-se a outros arquivos no seu repositório.

Imagens
Você pode exibir uma imagem adicionando ! e colocando o texto Alt entre [ ]. Em seguida, coloque o link da imagem entre parênteses ().

![This is an image](https://myoctocat.com/assets/images/base-octocat.svg)

Imagem interpretada

O GitHub dá suporte à inserção de imagens em problemas, solicitações de pull, discussões, comentários e arquivos .md. Você pode exibir uma imagem do seu repositório, adicionar um link para uma imagem on-line ou fazer o upload de uma imagem. Para obter mais informações, confira "Como carregar ativos".

Dica: quando você quiser exibir uma imagem que está no seu repositório, use links relativos em vez de links absolutos.

Aqui estão alguns exemplos para usar links relativos para exibir uma imagem.

Contexto	Link relativo
Em um arquivo .md no mesmo branch	/assets/images/electrocat.png
Em um arquivo .md em outro branch	/../main/assets/images/electrocat.png
Em problemas, pull requests e comentários do repositório	../blob/main/assets/images/electrocat.png?raw=true
Em um arquivo .md em outro repositório	/../../../../github/docs/blob/main/assets/images/electrocat.png
Em problemas, pull requests e comentários de outro repositório	../../../github/docs/blob/main/assets/images/electrocat.png?raw=true
Observação: os dois últimos links relativos da tabela acima funcionarão para imagens de um repositório privado somente se o visualizador tiver, pelo menos, acesso de leitura no repositório privado que contém essas imagens.

Para obter mais informações, confira Links relativos".

Especificando o tema para o qual uma imagem será exibida
Você pode especificar o tema para o qual uma imagem é exibida no Markdown usando o elemento HTML <picture> em combinação com o recurso de mídia prefers-color-scheme. Nós distinguimos entre os modos de cores claro e escuro. Portanto, há duas opções disponíveis. Você pode usar essas opções para exibir imagens otimizadas para fundos escuros ou claros. Isso é particularmente útil para imagens PNG transparentes.

Por exemplo, o seguinte código exibe uma imagem de sol para temas claros e uma lua para temas escuros:

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://user-images.githubusercontent.com/25423296/163456776-7f95b81a-f1ed-45f7-b7ab-8fa810d529fa.png">
  <source media="(prefers-color-scheme: light)" srcset="https://user-images.githubusercontent.com/25423296/163456779-a8556205-d0a5-45e2-ac17-42d089e3c3f8.png">
  <img alt="Shows an illustrated sun in light mode and a moon with stars in dark mode." src="https://user-images.githubusercontent.com/25423296/163456779-a8556205-d0a5-45e2-ac17-42d089e3c3f8.png">
</picture>
O método antigo de especificar imagens com base no tema, usando um fragmento acrescentado à URL (#gh-dark-mode-only ou #gh-light-mode-only), foi preterido e será removido em favor do novo método descrito acima.

Listas
Você pode criar uma lista não ordenada precedendo uma ou mais linhas de texto com -, * ou +.

- George Washington
* John Adams
+ Thomas Jefferson
Lista não ordenada renderizada

Para ordenar a lista, coloque um número na frente de cada linha.

1. James Madison
2. James Monroe
3. John Quincy Adams
Lista ordenada renderizada

Listas aninhadas
Você pode criar uma lista aninhada recuando um ou mais itens da lista abaixo de outro item.

Para criar uma lista aninhada usando o editor Web do GitHub ou um editor de texto que use uma fonte monoespaçada, como o Visual Studio Code, você pode alinhar a lista visualmente. Digite caracteres de espaço na frente do item de lista aninhada até que o caractere de marcador da lista (- ou *) fique diretamente abaixo do primeiro caractere do texto no item acima dele.

1. First list item
   - First nested list item
     - Second nested list item
Observação: no editor baseado na Web, você pode recuar uma ou mais linhas de texto ou desfazer o recuo realçando primeiro as linhas desejadas e, depois, usando Tab ou SHIFT+Tab, respectivamente.

Lista aninhada com alinhamento destacado

Lista com dois níveis de itens aninhados

Para criar uma lista aninhada no editor de comentários do GitHub, que não usa uma fonte monoespaçada, você pode observar o item da lista logo acima da lista aninhada e contar o número de caracteres que aparecem antes do conteúdo do item. Em seguida, digite esse número de caracteres de espaço na fonte do item da linha aninhada.

Neste exemplo, você pode adicionar um item de lista aninhada no item de lista 100. First list item recuando o item de lista aninhada no mínimo cinco espaços, pois há cinco caracteres (100. ) antes de First list item.

100. First list item
     - First nested list item
Lista com um item de lista aninhada

Você pode criar vários níveis de listas aninhadas usando o mesmo método. Por exemplo, como o primeiro item de lista aninhada tem sete caracteres (␣␣␣␣␣-␣) antes do conteúdo da lista aninhada First nested list item, você precisa recuar o segundo item de lista aninhada com sete espaços.

100. First list item
     - First nested list item
       - Second nested list item
Lista com dois níveis de itens aninhados

Para obter mais exemplos, confira a Especificação do GitHub Flavored Markdown.

Listas de tarefas
Para criar uma lista de tarefas, coloque um hífen e um espaço seguidos de [ ] antes dos itens de lista. Para marcar uma tarefa como concluída, use [x].

- [x] #739
- [ ] https://github.com/octo-org/octo-repo/issues/740
- [ ] Add delight to the experience when all tasks are complete :tada:
Lista de tarefas gerada

Se a descrição de um item da lista de tarefas começar com parênteses, você precisará fazer escape dele com \:

- [ ] \(Optional) Open a followup issue

Para obter mais informações, confira "Sobre listas de tarefas".

Mencionar pessoas e equipes
Você pode mencionar uma pessoa ou uma equipe no GitHub digitando @ mais seu nome de usuário ou o nome da equipe. Isto desencadeará uma notificação e chamará a sua atenção para a conversa. As pessoas também receberão uma notificação se você editar um comentário para mencionar o respectivo nome de usuário ou da equipe. Para obter mais informações sobre notificações, confira "Sobre notificações".

Observação: Uma pessoa será notificada sobre uma menção somente se ela tiver acesso de leitura ao repositório e, caso o repositório pertença a uma organização, se ela for membro da organização.

@github/support What do you think about these updates?

@mention renderizado

Quando você menciona uma equipe principal, os integrantes de suas equipes secundárias também recebem notificações, simplificando a comunicação com vários grupos de pessoas. Para obter mais informações, confira "Sobre equipes".

Se você digitar um símbolo @, uma lista de pessoas ou de equipes em um projeto será exibida. A lista é filtrada à medida que você digita. Portanto, assim que você achar o nome da pessoa ou da equipe que está procurando, use as teclas de seta para selecioná-lo e pressione tab ou enter para completar o nome. Para equipes, insira o @organization/team-name e todos os membros dessa equipe serão inscritos na conversa.

Os resultados do preenchimento automático são restritos aos colaboradores do repositório e qualquer outro participante no thread.

Fazer referências a problemas e pull requests
Você pode mostrar uma lista de solicitações de pull e problemas sugeridos no repositório digitando #. Digite o número ou o título do problema ou da pull request para filtrar a lista e, em seguida, pressione tab ou enter para completar o resultado destacado.

Para obter mais informações, confira "URLs e referências autovinculadas".

Fazer referência a recursos externos
Se as referências de link automático personalizado estão configuradas para um repositório, referências a recursos externos, como um problema do JIRA ou um ticket do Zendesk, serão convertidas em links encurtados. Para saber quais links automáticos estão disponíveis no repositório, entre em contato com alguém com permissões de administrador no repositório. Para obter mais informações, confira "Configurar links automáticos para fazer referência a recursos externos".

Fazer upload de ativos
Você pode fazer upload de ativos como imagens, arrastando e soltando, fazendo a seleção a partir de um navegador de arquivos ou colando. Carregue ativos em problemas, solicitações de pull, comentários e arquivos .md no seu repositório.

Usar emoji
Adicione um emoji à sua escrita digitando :EMOJICODE:.

@octocat :+1: This PR looks great - it's ready to merge! :shipit:

Emoji renderizado

Se você digitar :, uma lista de emojis sugeridos será exibida. A lista será filtrada à medida que você digitar algo. Portanto, assim que encontrar o emoji que estava procurando, pressione Tab ou ENTER para completar o resultado realçado.

Para obter uma lista completa de emojis e códigos disponíveis, confira a Emoji-Cheat-Sheet.

Parágrafos
Você pode criar um parágrafo deixando uma linha em branco entre as linhas de texto.

Notas de rodapé
Você pode adicionar notas de rodapé ao seu conteúdo usando esta sintaxe entre colchetes:

Here is a simple footnote[^1].

A footnote can also have multiple lines[^2].

You can also use words, to fit your writing style more closely[^note].

[^1]: My reference.
[^2]: Every new line should be prefixed with 2 spaces.
  This allows you to have a footnote with multiple lines.
[^note]:
    Named footnotes will still render with numbers instead of the text but allow easier identification and linking.
    This footnote also has been made with a different syntax using 4 spaces for new lines.
A nota de rodapé será interpretada da seguinte forma:

Nota de rodapé interpretada

Observação: a posição de uma nota de rodapé no Markdown não influenciará o lugar em que a nota de rodapé será renderizada. Você pode escrever uma nota de rodapé logo após sua referência à nota de rodapé, e ela continuará sendo interpretada na parte inferior do Markdown.

Não há suporte para notas de rodapé em wikis.

Ocultando o conteúdo com comentários
Você pode dizer a GitHub para ocultar o conteúdo do markdown interpretado, colocando o conteúdo em um comentário HTML.

<!-- This content will not appear in the rendered Markdown -->
Ignorar formatação markdown
Instrua o GitHub a ignorar a formatação Markdown (ou fazer escape dela) usando \ antes do caractere Markdown.

Let's rename \*our-new-project\* to \*our-old-project\*.

Caractere com escape renderizado

Para obter mais informações, confira "Sintaxe de Markdown" do Daring Fireball.

Desabilitando a interpretação do Markdown
Ao visualizar um arquivo Markdown, você pode clicar em  na parte superior do arquivo para desabilitar a renderização do Markdown e ver a origem do arquivo.

Captura de tela de um arquivo Markdown em um repositório do GitHub mostrando as opções para interagir com o arquivo. Há um botão para exibir o blob de origem com um contorno em laranja escuro.

Se você desabilitar a renderização do Markdown, poderá usar recursos de exibição de origem, como vinculação de linha, o que não é possível ao exibir arquivos Markdown renderizados.

Leitura adicional