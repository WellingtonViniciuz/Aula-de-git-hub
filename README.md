# O que é Markdown?

O Markdown é uma linguagem de marcação leve e fácil de usar, criada em 2004. Ela permite formatar textos (como colocar palavras em negrito, criar listas ou títulos) usando símbolos simples do teclado. O objetivo é escrever de forma rápida, mantendo o texto legível em sua forma pura e podendo ser convertido para HTML.

## Dois asteriscos (\*\*), são o código markdown para texto em negrito.

**negrito**

## Um pouco mais de código, por favor.

Vamos começar usando os códigos para o título:

**OBS** Na sintaxe Markdown, a hierarquia e o tamanho do título são definidos pela quantidade sequencial do caractere de cerquilha (#)

# Título 1 

## Título 2 

### Título 3

#### Título 4

##### Título 5

###### Título 6

# Ênfase no documento

Para adicionar ênfase ao conteúdo que será escrito, usamos o asterisco \* ou (_underline_)\_:

### Veja como é simples:

**negrito** Usando (\**)
*itálico* Usando (*)

## Links

Existem duas formas de inserir um link em Markdown. Através de um link direto ou um texto-âncora:

### Texto âncora

Utilizamos os caracteres [] (), dentro da chave o texto e dentro do parêntese o link, exemplo:

[LinkedIn](https://www.linkedin.com/in/wellington-vinicius-jiudev)

### Link direto

Coloque o endereço URL dentro de chaves, exemplo:
<https://www.linkedin.com/in/wellington-vinicius-jiudev>

## Lista de itens

Para listas não ordenadas, utilize um asterisco \* na frente do item:

* item 1
* item 2
* item 3

## Para listas ordenadas, utilize:

1. Item 1
2. Item 2
3. Item 3

## As listas acima serão exibidas desta forma:

- Não Ordenada 1
- Não Ordenada 2

1. Ordenada 1
2. Ordenada 2

## Imagens

O código para inserir uma imagem no conteúdo é semelhante ao código de inserir links-âncora. Adicionando apenas um ponto de exclamação à frente, exemplo:

![título da imagem](https://media.licdn.com/dms/image/v2/C4D12AQE0MGUjGNxTJg/article-cover_image-shrink_720_1280/article-cover_image-shrink_720_1280/0/1653237867013?e=1783555200&v=beta&t=FAJMapoS9Rf-Fmh9Oy0Zx4Ht_858udiv6x0zAO8HY50)

## Citação (Quote)

Para transformar um bloco de texto em uma citação, ou comentário, coloque o caractere > à frente, exemplo:

> A vida é boa e sempre vai dar certo

## Colocando código no texto

Há dois modos de adicionar trechos de código em Markdown. O primeiro é colocar o código em uma linha, e o outro é colocar em múltiplas linhas.

Para colocar um código em uma linha, utilize o acento grave ` no início e no final do código:

`Codigo aqui`

### Para múltiplas linhas, coloque três acentos graves (``` ):

```

Primeira linha do código
Segunda linha do código
Terceira linha do código

```
# Padrões de Commits (Commit Patterns)
É de muita importância que todos os envolvidos no projeto entendam as mudanças ocorridas e quais foram os contextos de alteração do código. Para isso o __git commit__ precisa ser utilizado apropriadamente



## O que é o Conventional Commits ?

O Conventional Commits é uma convenção simples de mensagens de commit, que segue um conjunto de regras e que ajuda os projetos a terem um histórico de commit explícito e bem estruturado.

O **Conventional Commits** deixara a linha do tempo de um projeto mais estruturada e fácil de entender. Quando documentados utilizando o **Conventional Commits** nos mostram quem alterou, quando, em qual contexto e qual tipo de alteração foi feita.

## Como utilizar ?
A mensagem do commit deve ser estruturada da seguinte forma:

```
:emoji: <tipo>(escopo): <descrição>

```
Os commits terão um emoji para dar uma identificação visual a mensagem, um tipo, um escopo para dar contexto, e uma descrição onde poderá colocar os detalhes do commit.

**OBS**: O emoji e o escopo são opcionais, porém é recomendado que siga o escopo a cima.

## Tipos de Commits

O commit possui os elementos estruturais abaixo (tipos), que informam a intenção do seu commit ao utilizador(a) de seu código.

* **fix** - Commits do tipo fix indicam que seu trecho de código commitado está solucionando um problema (bug fix), (se relaciona com o PATCH do versionamento semântico).

* **feat**- Commits do tipo feat indicam que seu trecho de código está incluindo um novo recurso (se relaciona com o MINOR do versionamento semântico).

* **docs** - Commits do tipo docs indicam que houveram mudanças na documentação, como por exemplo no Readme do seu repositório. (Não inclui alterações em código).

* **style** - Commits do tipo style indicam que houveram alterações referentes a formatações de código, semicolons, trailing spaces, lint... (Não inclui alterações em código).

* **refactor** - Commits do tipo refactor referem-se a mudanças devido a refatorações que não alterem sua funcionalidade, como por exemplo, uma alteração no formato como é processada determinada parte da tela, mas que manteve a mesma funcionalidade, ou melhorias de performance devido a um code review.

* **build** - Commits do tipo build são utilizados quando são realizadas modificações em arquivos de build e dependências.

* **test** - Commits do tipo test são utilizados quando são realizadas alterações em testes, seja criando, alterando ou excluindo testes unitários. (Não inclui alterações em código)

* **chore** - Commits do tipo chore indicam atualizações de tarefas de build, configurações de administrador, pacotes... como por exemplo adicionar um pacote no gitignore. (Não inclui alterações em código)

## Emojis
| Tipo de Commit | Emoji e Código |
| :--- | :--- |
| Commit inicial | 🎉 `:tada:` |
| Tag de versão | 🔖 `:bookmark:` |
| Novo recurso | ✨ `:sparkles:` |
| Lista de ideias (tasks) | 🔜 `:soon:` |
| Bugfix | 🐛 `:bug:` |
| Documentação | 📚 `:books:` |
| Testes | 🧪 `:test_tube:` |
| Adicionando um teste | ✅ `:white_check_mark:` |
| Teste de aprovação | ✔️ `:heavy_check_mark:` |
| Acessibilidade | ♿ `:wheelchair:` |
| Texto | 📝 `:pencil:` |
| Package.json em JS | 📦 `:package:` |
| Em progresso | 🚧 `:construction:` |
| Arquivos de configuração | 🔧 `:wrench:` |
| Removendo uma dependência | ➖ `:heavy_minus_sign:` |
| Adicionando uma dependência | ➕ `:heavy_plus_sign:` |
| Revertendo mudanças | 💥 `:boom:` |
| Alterações de revisão de código | 👌 `:ok_hand:` |
| Refatoração | ♻️ `:recycle:` |
| Mover/Renomear | 🚚 `:truck:` |

## Exemplos de utilização

git commit -m ":tada: Iniciando projeto"
git commit -m ":heavy_plus_sign: build: Instalando dependencias"
git commit -m ":sparkles: feat(header): Adicionando e posicionando os icones"
git commit -m ":books: docs(readme): Criando documentação do projeto"

# Atenção
**_Algumas partes deste artigo como por exemplo o uso de emojis é uma particularidade não necessariamente é o mais certo a se fazer, muitas empresas usam padrões de commits diferentes. O importante é se atentar ao escrever a mensagem de um commit, para que outros entendam e fique bem claro oque foi alterado ou criado_**

## Referências e Leituras Recomendadas

* **Padrões de Commits:** Grande parte da seção sobre regras e tipos de commits foi baseada neste [Artigo de Apoio no Dev.to](https://dev.to/renatoadorno/padroes-de-commits-commit-patterns-41co).
* **Conventional Commits:** [Site Oficial](https://www.conventionalcommits.org/en/v1.0.0/)