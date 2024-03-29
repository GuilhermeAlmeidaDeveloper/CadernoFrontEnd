
# Módulo 2

# Introdução ao Front-End e a Web.

1- O que é front-end?

O back-end possui muito mais dados sensíveis que o front-end. O front é processado pelo dispositivo do cliente.

2- Quais os tipos de clientes?

- Mobile (apple e android)
- Desktop (notbook ou gabinete)
- Outros (SmartWatchs, SmartTV, Painel de Shopping, Maquina de cartão de crédito)

3- Quais os tipos de sistemas operacionais (software que te dá uma estrutra de acessar a internet e diversas outras funcionalidades).

- IOS, Android
- Windows, Linux, MACos

4- Maneiras de desenvolver um software:
- Nativo
- Multiplataforma

Nativo:
Usa-se uma linguagem do programação que interage diretamente com o hardware, são rápidas, tem acesso a todas as funcionalidades do dispositivo. Precisam ser refeitas para que rode em outro sistema Operacional.

Swift e Objective-C (IOS e MACos);
Java e Kotlin (Android);
C# (Windows);

Multiplataformas:
Funcionam em 2 ou mais plataformas, evitando retrabalho. Não costumam ter acesso as funcionalidades do despositivo e não costumam ter a mesma velocidade.

A forma mais comum de se fazer aplicações multiplataforma é usando a Web.

Mas o que é a web?

Como funciona a internet?

Existe o cliente (dispositivo que se conecta com a internet), que se conecta com a rede mundial de computadores (net) e por fim os servidores, onde guardamos informações, sejam eles sites, fazemos upload de arquivos e etc.

DNS - Coloca 'apelidos' nos sites. Um IP é um número de identificação de um site, e com o DNS é possível substituir o número pelo nome para acessá-lo.

O que são navegadores?
São programas que intepretam sites.
HTML - Linguagem de Marcação
CSS - Estilização do site
Javascript - Vai dar funcionalidade ao Site.

Especificação
Define uma linguagem, determinando:
- Como ela se escreve.
- Como ela é executada.
.

# Aula 2

# Tags, Atributos e Valores

As tags são quase impossíveis de decorar de cara, são muitas. Com a prática, iremos entende-las melhor.

HTML siginifica Linguagem de Hipermarcação de Texto.

É uma linguagem usada para criação de websites, é usada para definir a estrutura do seu conteúdo.

''<! DOCTYPE html>'' - informa para o arquivo que o tipo dele é html;

''< html> - Tag raiz, que engloba todas as outras;

''< META > - tag que define metados, informações sobre os dados do documento html (fica dentro do head);

''< head>'' - São configurações que instauramos no documento (também não aparece para o usuário);

''< body>'' - Informações que de fato aparecem para os usuários.

Tag siginifica etiqueta, em html elas demarcam conteúdo.

Estrutura:( < p> ) tag de abertura  , 'olá mundo conteudo' e (</ p> ) tag de fechamento

Uma TAG com tag de abertura, tag de fechamento, propriedade, conteúdo forma um ELEMENTO do html.

ESTUDAR AS ESPÉCIEIS DE TAGS NO MDN*

Tags importantes:

div - cria um container, funciona como divisor para agrupar outras tags html dentro (exemplo da escola e salas). É possivel ter tags dentro de tags, ou seja existem outras tags dentro dos divs.

ol - cria uma lista ordenada

ul - cria uma lista não ordenada

li - adiciona uma linha na lista

Algumas tags possuem a característa self-closing, ou seja, elas se fecham sozinhas e não precisam ser fechadas, como por exemplo a tag < img>.

img também possui o que chamamos de propriedade, no caso scr=.

Conceito Arvore HTML*

Para colocar uma imagem no meu site, ela deve estar necessáriamente na pasta do projeto do site, pq no futuro, ao subir os arquivos para o servidor, se a img nao estiver na pasta, ele nao vai encontrar depois.

# AULA 3

## CSS: Propósito, seletores e propriedades.

Css é uma linguagem de estilos, escritas que adiciona estilos aos elementos do HTML

Os códigos do CSS são divididos em Seletores, Propriedades e Valores.

seletor {
    propriedade: valor;
}

h1 {
    color: red
}

Seletor: responsável por selecionar o elemento que será estilizado.

Propriedade: Diz o que será alterado no elemento selecionado.

Valor: o que vai variar na propriedade.

Dentre os seletores, existe diversos:

O universal: representado pelo asterisco *

O próprio elemento: h1, h2, p, div.

A Classe: representado por .nome-da-classe

o ID: representado por #nome-do-ID.

Utiliza-se /* para comentar um código em css/html */

Cascata = o que tá em baixo tem mais prioridade.

O css pode ser escrito de três maneiras:

Inline, diretamente no elemento html

Dentro da tag < style>, essa tag fica dentro da tag head do arquivo HTML.

Ou em um arquivo externo, essa arquivo deve ter a extensão .css. (utiliza-se a tag < link rel='stylesheet' href = ''style.css''>)

Ordem de prioridade:

O CSS inline tem mais poder, posteriormente vem o arquivo/tag style, dependendo da ordem que aparecer a tag style ou a importação do arquivo por conta da CASCATA.

Unidades de madidas:

- em

- rem

- px

- cm 

- %

Em primeiro momento usaremos a % e o px.

*Estudando combinação de seletores (classe, ID e elemento.)

## Box Model

Todos os elementos do HTML podem ser considerados uma box, por isso ela tem lados e possibilidade de alterar propriedades.

A div/h1 tem como propriedades:

Conteúdo, padding (espaçamento interno), border, margin (espaçamento do elemento para outro elemento).

## Elementos INLINE e BLOCK.

Existem elemetnos de bloco e de linha, eles funcionam diferentes um do outro, resumidamente:

- Bloco : Ocupa a largura total da página.

- Linha : Ocupa apenas o tamanho necessário para o elemento.

# AULA 4

CSS: Propriedades e mais regras de funcionamento.

- Herança

- Pseudos

- Combinadores 

- Propriedades de Texto

- Cores

- Listas 

- Sombras

- Background-image

- Bordas

## Herança

No css, os elementos herdam algumas propriedades de seus parentes, não sao todas, mas algumas delas.

## Pseudos (selecinados com ::)

Existem elementos no HTML que possuem várias partes para serem estilizadas, por isso foram criados pseudo-elementos, que nos ajudam a estilizar um elemento por partes. Principais pseudo-elementos: After/Before/Placeholder/backdrop.

## Pseudos-Classes. (selecinados com :)

Permitem que o css observe o estado atual de um elemento, por exemplo:

- Quando um usuário passa o ouse em cima do elemento;

- Quando um link já foi visitado

- Quando um elemento está selecionado

- Quando um elemento é o primeiro filho de um pai.

Ex: Hover, active, visited, focus, first-child, last-child.

## Combinadores de seletores:

Já aprendemos a selecionar os elementos do html no css atraves do:

- Nome do elemento, ex: h1

- ID do elemento, ex: #códigodoid

- Pela classe, ex: .nomedaclasse

Podemos combinar os seletores, por exemplo:

elemento1 elemento2 : Vai selecionar todo e qualquer elemento2 que estiver dentro do elemento1

elemento1 + elemento2: Vai selecionar qualquer elemento2 que segue imediamentamente após um elemento ul

elemento1 ~ elemento2: Vai selecionar todos os elementos do tipo elemento2 que seguir o elemento dentro de um mesmo elemento pai

elemento1 > elemento2: Ira selecionar todos os elemento2 que estiverem diretamente dentro do elemento1

## Cores

- Cores nomeadas: white, black, purple.

- Cores Hexadecimais: #0000ffff

- RGB: combinação de red green e blue

-HSL: Cores com base na percepção humana, combina matriz, saturação e luminancia.

## Propriedade para texto:

- Text-align: Alinha o texto

- Text-decoraction: adciona uma decoração ao texto.

- Font-family: Modifica a fonte padrao

- Font-size: Modifica o tamanho da font

- Font-Transformation: uppercase, lowercase.

# Aula 4

Vamos entender um pouco sobre Viewport.

Viewport consiste em toda a área útil do navegador, ou seja, somente onde o site é exibido, descontando tamanho de barras de navegação, ferramentas do desenvolvedor e etc.

Nos temos o viewport height e viewport width.

Essas medidas também podem ser usadas para definir a autura e largura de elementos.

vw= 1% da viewport width
100vw = 100% da viewport width
vh= 1% da viewport high
100vh = 100% da viewport high

Mas o que é layout?

"Modo de distribuição e arranjo dos elementos gráficos num determinado espaço ou superfície."

No CSS, existem diversos tipos de layouts, os principais são:

- Normal-flow
- Flex-box 
- Grid

Nessa aula trataremos do normal-flow, o layout Padrao default do CSS.

## Elementos de block e inline.

Por padrao, um elemento de block, é 100% da largura do elemento pai, e tão alto quanto o seu conteúdo exige.

Enquanto um elemento inline, ocupa apenas a largura e altura necessária para o conteúdo ser exibido.

Layouts Adptativos>

São layouts que se adptam tanto para PC quanto para Mobile.

O layout responsivo é aquele se adpta exatamente a uma tela de qualquer dispositivo, com as melhores usabilidades para aquele dispositivo.

Já o layout Fluido, ele é criado de forma que possa ser utilizado em qualquer dispositivo, porém ele nem sempre tem as melhores regras e usabilidade.

## Conceito de Container.

No frontEnd, um container é algo que envelopa outras coisas, por exemplo:

Uma ul tem varias LI, logo essa ul é um container para li.

## Positions

Existem propriedades que nos ajudam a posicionar, elas são os positions, nós temos algumas variações:

-static

-relative

-absolute

-fixed

-sticky

## Z-INDEX

Também é uma maneira de posicionar elementos.

Quando estamos posicionando um elemento na horizontal, utilizamos o eixo X, quando é na vertical, utilizamos o eixo Y.

Agoar quando queremos determinar a profundidade dos elementos, qm fica na frente de qm, utilizamos o z-index.

Será sempre definido como um valor inteiro, seja ele negativo ou positivo.