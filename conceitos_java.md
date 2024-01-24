# Conceitos Básicos do Java
Neste documento estarão informações básicas e teóricas a respeito da linguagem Java

## Visão geral do Java

Como muitas outras linguagens, Java é uma linguagem de programação cujos aspectos possuem relação entre suas outras características. Por isso, é necessário entender antes alguns conceitos básicos da linguagem para melhor compreender cada aspecto. Eis os principais aspectos da linguagem Java.

### Orientação a Objetos

Não é possível falar em Java sem falar de Orientação a Objetos, sendo uma linguagem de extrema força nesse paradigma. A Orientação a Objetos é o núcleo do Java. É inclusive importante, antes de estudar a linguagem, estudar o paradigma POO para não temer a linguagem. Serão especificados a seguir alguns princípios básicos desse paradigma.

#### Dois paradigmas

Ao lidar com a criação de um programa, pode-se tomar a decisão de escolher entre dois principais "paradigmas": formular o programa baseado em seu código estruturado ou construir o programa de acordo com os dados que são fornecidos. 

O modelo orientado a processos ou paradima procedural é o que condiz com o embasamento no código, criando-se programas lineares e estruturados cujos códigos agem sobre os dados. Exemplo de linguagem nesse sentido é o próprio C. O principal problema, porém, desse paradigma, como já se viu em outros documentos, é o tamanho e a complexidade dos programas.

Com o intuito de gerenciar essa complexidade, existe a segunda aproximação que é a Programação Orientada a Objetos (POO). Diferente do primeiro, organiza o código baseado nos seus dados e define interfaces para se chegar a esses dados. Seu principal ponto está em os dados controlar o acesso ao código, o que traz diversos benefícios organizacionais.

##### Abstração

A abstração é essencial na POO. Consiste na redução dos detalhes para focar naquilo que é necessário. Isto é frequentemente feito por nós seres humanos. Por exemplo, quando se pensa em um animal, suponha-se um cachorro, logo se imagina um animal peludo, de diferentes raças, altura mais ou menos na cintura, e se destaca sobre o seu comportamento: alegre, raivoso, latir, carinhoso, etc. 

A questão é que, para imaginar o animal, não se pensa em cada parte separada até se completar o todo. Como assim? Não pensamos nas células que compõem o animal, depois seus tecidos, seus órgãos, sistemas, até chegar na imagem mental comum que se tem na mente. Ou seja, somente se enxerga aquilo que se necessita naquele momento, a imagem do cachorro, porém ao analisar o seu interior verá que é algo muito mais complexo.

Essa abstração justamente utiliza uma organização hierarquical para dividir e gerenciar o programa. O cachorro, de maneira superficial, possui um corpo, mas dentro desse corpo estão sistemas, que por sua vez possuem órgãos, os quais são formados por tecidos que são constituídos por células, e por ái vai. Então esse princípio define a subdivisão do objeto em outros objetos de forma a torná-lo mais simples e focar no que é necessário ao problema.

Isto obviamente pode ser aplicado a programas de computador. A abstração pode transformar as instruções de um programa do modelo baseado em processos (ou paradigma procedural) em seus objetos componentes. Estes objetos, que possuem seu próprio comportamento, irão se relacionar por meio de mensagens as quais irão comandar e instruí-los o que fazer.

#### Encapsulamento

É o mecanismo da POO que isola os elementos de um objeto para que não sejam interferidos por outros objetos ou métodos, por interferência externa ou descuido. Vale-se analisar o encapsulamento como uma "embalagem" que impede do código e seus dados serem acessados por outros códigos. E esse acesso aos componentes internos ocorre mediante uma interface bem definida.

Veja-se um exemplo a respeito desse princípio. Imagine o sistema de freios de uma bicicleta. Esse sistema somente pode ser interferido ou acessado quando você utilizar os freios, de sorte que os pedais de aceleração, a buzina ou os faróis da bicicleta não interferirão nesse sistema. Assim é o que acontece com o encapsulamento, isolando os componentes de um objeto por meio de uma interface, um método no qual se acessa a entidade. 

Agora, esse sistema de freios pode ser diferente para diversos fabricantes de bicicleta, porém ao fim das contas o resultado é o mesmo para o usuário: apertar o freio desacelera a bicicleta até parar ou retirar a mão do freio.

Então o ponto principal do encapsulamento é acessar os objetos por meio de uma interface, executando suas funções e comportamentos mesmo sem saber de seus detalhes internos.

##### Classes

A base do encapsulamento é a classe. Define-se como uma estrutura de atributos (variáveis) e métodos (funções) que servirão de base para uma série de objetos. Os objetos são moldados à classe e por isso podem ser chamados de instâncias dessas classes. Em outras palavras, a classe é um projeto lógico, os objetos são sua representação em realidade.

Criando sua classe, são definidos seus atributos e métodos (dados e código). Os dados que serão definidos para essa classe, imaginando um exemplo de um carro, são seus atributos: cor, tamanho, velocidade máxima, caronagem, modelo do carro, do motor, etc. Já os comportamentos dessa classe, o código que opera mudando essas características, como por exemplo ligar carro, acelerar, freiar, são os métodos.

Desde que o propósito de uma classe é encapsular a complexidade do programa, existem elementos que possibilitam ocultar as implementações complexas dentro dessas estruturas. Dessa forma, os atributos ou métodos de uma classe podem ser destacados como *público* ou *privado*. 

A interface pública de uma classe representa tudo o que os usuários externos sabem ou podem saber da mesma. Já atributos e métodos privados podem ser somente acessados a partir da classe em que se encontram, de forma que códigos externos não podem interferir nesses elementos.

Assegura-se então que essas características privadas sejam somente acessadas pelos métodos públicos dessa classe, para que nenhum outro código as tenha acesso. Isso, portanto, implica que seu código deve ser construído no intuito de não expor funcionamentos internos de sua classe.

#### Herança

Herança é o processo no qual um objeto herda características de outro objeto. Isso é importante para a organização hierarquical e a reutilização de código. Como exemplo, imagine-se um jabuti. O jabuti é um *animal* da classe *réptil*. A herança nesse caso ocorre da seguinte maneira: a classe animal possui dentre outros exemplos atributos como idade, sexo, peso, está vivo, se possui pelos, tipo de sistema esquelético, forma de locomoção e outras características; e métodos como comer, beber, dormir, respirar. Já a classe réptil possui todas essas características adicionadas a atributos do tipo: sangue frio, se possui ecdise (troca de pele), se possui casco, se possui peçonha; métodos como disfarçar-se com o ambiente, trocar pele a cada x tempo, injetar veneno sobre presa, etc.

Essa herança no caso do objeto jabuti ocorre a partir da classe réptil herdar atributos e métodos da *superclasse* animal. Esta classe réptil por sua vez é *subclasse* de animal, que pode ser superclasse de outra classe, como por exemplo para Testudines (Ordem do Jabuti), que pode ser para Testudinidae (Família do Jabuti), e por aí vai.

Simplesmente, então, a herança é o método com o qual os objetos específicos herdarão características de objetos gerais, reutilizando código.

##### Polimorfismo

Palavra que provém do grego, significa *muitas formas*. Basicamente define os contextos em que uma única interface pode agir em uma classe de métodos. O método entra em ação dada a natureza exata do contexto. Tome como exemplo um programa que realiza soma dois *dados*. Na entrada do usuário, pode ocorrer principalmente 4 possibilidades: o utilizador digitar dois inteiros, dois doubles, dois caracteres ou duas strings. O polimorfismo então envolve essas situações na classe de métodos para atender ao resultado esperado, o de realizar a soma dos dados digitados, seja número ou literal. 

Em uma linguagem de programação sem orientação a objetos seria necessário criar 4 funções com nomes diferentes para aplicar a devida operação nos dados. Além de tudo, precisaria criar condicionais para executar cada função baseado no tipo do dado digitado. Porém com a POO é possivel criar métodos de mesmo nome para executar as operações esperadas pelo usuário, sem a necessidade de criar condicionais para os tipos de dados. 

Resume-se então o polimorfismo na frase "uma interface, múltiplos métodos". Ou seja, a definição de uma interface que, dados os diferentes contextos de entrada do usuário, leva a métodos para cada uma dessas situações, criados em uma classe genérica de métodos.

## Elementos gerais da linguagem Java

Aqui será discorrido com relação a elementos simples da linguagem Java. 

### Espaço em branco

A linguagem Java não segue uma regra restrita sobre identação. Isto significa que você pode escrever todo o seu código em uma única linha, desde que cada instrução esteja separada por um espaço.

### Identificadores

Outro elemento interessante utilizado em qualquer lugar da linguagem Java são os identificadores, nomes os quais se dão a variáveis, classes, métodos, etc. Estes nomes sempre seguem um padrão. Tais identificadores não podem começar por números, nem possuir nomes de palavras-chave da linguagem ou símbolos utilizados para algo, como +, -, *, {, } e outros caracteres especiais. 

### Separadores

São caracteres que separam e agrupam dados, métodos, informações e outras coisas. Veja alguns a seguir:

Separador | Função 
--- | ---
";" | Determina o fim de uma instrução ou estado, ao possibilitar a execução da próxima caso haja.
"{ }" | Definem um bloco de código para estruturas de repetição, condicionais, métodos, classes e outras entidades. Também são importantes para a criação de Arrays.



