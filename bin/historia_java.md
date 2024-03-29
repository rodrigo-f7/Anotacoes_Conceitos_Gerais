# História do Java

Entender sobre os processos passados antes de aprender algo é fundamental. Por isso esse tópico se dedicará totalmente para destacar um pouco da história do Java, como ele se desenvolveu e qual o seu propósito, de maneira resumida e objetiva.

## Linhagem do Java
Java é uma linguagem de programação orientada a objetos com sintaxe influenciada das linguagens de programação C e C++. Muito de sua sintaxe advém da linguagem C, enquanto que os fundamentos da OOP vêm de grande parte da linguagem C++. Como muitas linguagem de programação, o Java veio com o intuito de resolver problemas que seus anteriores não conseguiam, no caso, problemas que as linguagens C e C++ enfrentavam.

### Sobre a Linguagem C

* Linguagem Estruturada, Poderosa e Eficiente
* Surgiu por volta dos anos 70 influenciada pelas Linguagens B e BCPL
* Não era tão difícil de aprender quanto Assembly em sua época e era mais eficiente do que BASIC
* Revolucionou a área da programação

### Sobre a Linguagem C++

* Chegou-se o limite das linguagens de programação estruturadas: muitos projetos de grande porte acabam ficando difíceis de entender com essas linguagens
* Surgimento de um novo paradigma de programação: Paradigma de Orientação a Objetos
* Criado C++ na Bell Laboratories por Bjarne Stroustrup em 1979
* Baseada em C, porém com implementações da programação Orientada a Objetos

## O Surgimento do Java
A linguagem de programação Java foi criado pela Equipe de James Gosling na empresa Sun MicroSystems no ano de 1991. Inicialmente chamada de Oak, seu nome foi somente efetivizado em 1995. Apesar de que a sua maior importância hoje em dia seja no Back-End e na Web, Java em seu período de criação possuía outras motivações.

Na verdade, o objetivo inicial do Java era criar uma linguagem de plataforma independente e eficiente capaz de executar instruções de CPUs controladoras em dispositivos eletrodomésticos, como controles remotos e microondas.

Isto foi necessário pois as linguagens C e C++ foram compiladas para propósitos específicos, sendo preciso compilar a linguagem para a incrementação em dispositivos diferentes, o que consumia tempo e esforço. A solução mais prática portanto era criar uma linguagem que possibilitava rodar em uma variedade de CPUs.

Embora tenha sido esta sua meta inicial, executando-a de maneira eficiente, o Java continuou obscuro para as empresas de eletrônicos e não fez sucesso por um tempo. Porém, com o advento da Internet, esta linguagem viu a oportunidade para agir novamente, já que, com todas as conexões feitas entre os computadores, era necessário haver uma linguagem que se era compreendida por todos esses computadores, ou seja, portátil, de plataforma independente.

E assim o Java conseguiu o seu sucesso, enquanto que inicialmente nasceu para criar programas embarcados em eletrônicos, agora o Java renasce no intuito de resolver o problema da Internet, auxiliando no processo de portabilidade de código na WWW.

A despeito de ser semelhante à linguagem C++, o Java não pode ser chamado de uma "extensão" dessa linguagem para a Internet. Criadas com propósitos diferentes, o Java conseguiu aprimorar princípios da POO (Programação Orientada a Objetos), possibilitou o uso de multithreading e a aplicação de classes que facilitam o acesso à Internet.

## O Impacto do Java na Internet

Os principais impactos do Java com a WWW foram com os Applets, a Segurança e a Portabilidade.

### Applets

Os applets eram pequenos programas rodados em navegadores compatíveis com o Java Web que executavam funções simples como exibir dados do servidor, receber dados do usuário, criar calculadores simples, etc.
Eles, então, àquele tempo, foram fundamentais para a circulação das informações e para explorar uma outra dimensão das páginas web. Porém sua derrocada chegou na Web, apesar de que, hodiernamente, poucas aplicações ainda utilizam applets, seu suporte foi finalmente finalizado com o JDK 11.

### Segurança

Com a construção processual da Internet, uma atividade muito comum reproduzida nela eram os Downloads. Baixar um programa na Internet representava "inserir" uma série de códigos em sua máquina, o que podia ocorrer em um ou mais desses códigos ser malicioso e danoso ao computador do cliente, um exemplos deles são vírus, cavalos de Tróia, Spywares e outros programas prejudiciais.
Assim, o Java nesse sentido vem para, com suas ferramentas e aparatos, isolar as aplicações em seu ambiente de execução para serem testadas sem danificar o sistema do usuário, verificando se aquela aplicação possui algum problema ou código perigoso.

### Portabilidade

Princípio básico do Java, sendo uma linguagem de plataforma independente, o Java foi fundamental para haver a conexão entre os computadores, que possuem diferentes CPUs e Sistemas Operacionais. É muito mais prático ter um programa na mesma versão rodando em vários computadores da Internet a ter várias versões do mesmo espalhados por não possuir compatibilidade com processadores, navegadores ou Sistemas Operacionais diferentes. Por isso, o Java é egrégio para manter um ambiente prático e dinâmico de execução das aplicações.

## ByteCode

O ponto chave do Java são os seus ByteCodes, que subsidiaram a resolução dos problemas da segurança e da portabilidade no ciberespaço. Eles são séries de instruções altamente otimizadas construídas para serem executadas na JVM (Java Virtual Machine ou Máquina Virtual Java), a qual faz parte do JRE (Java Runtime Environment).

Essencialmente, foi planejada como uma linguagem interpretada, o que pode parecer estranho para alguns pois uma linguagem interpretada possui complicações de performance, porém com a JVM e a criação dos bytecodes, bem como a utilização de técnicas de otimização de código como o HotSpot, torna-se viável e eficiente a execução dos programas.

Para rodar os programas, o Java utiliza a JVM com o JRE para encapsular a aplicação em seu ambiente de execução. Esta máquina virtual vai proporcionar o mesmo programa ser interpretado em computadores diferentes, bastando ao computador ter a JRE instalada que assim poderá executar o programa. Por isso, é muito dinâmico e portátil a execução dos programas em Java, sem ser necessário de recompilar o código para diversas plataformas, computadores e SOs.

Também a JVM é fundamental no sentido da segurança, pois possibilita a criação de um local de execução de programas isolado de todo o sistema: a chamada Sandbox, que proporciona testes e verificações de programas evitando violações do sistemas

É claro que, mesmo sendo uma linguagem "interpretada", caso seja necessário ou desejado, os bytecodes do Java podem ser compilados sem problemas para proporcionar melhor desempenho do programa. Muitas técnicas, como o HotSpot, já realizam isso, compilando as partes necessárias do código para aumentar a sua performance. 

## Sucessores dos Applets

Algumas décadas atrás era necessário a utilização dos applets para integrar na Web as aplicações Java. Com o tempo os applets foram perdendo suporte, sendo finalizados a partir da JDK 11. Porém a integração da Web não havia acabado: com a criação do Java Web Start, era possível colocar apps Java na Web por meio de um cliente externo, uma aplicação baixada do navegador e aberta no sistema. Contudo, ao longo do tempo, estes também foram perdendo suporte. Acontece que todas essas funcionalidades do Java ainda existem e podem ser utilizadas, porém dada a defasagem acaba se tornando obsoleto os seus usos.

## Fluxo de Atualizações

Há anos atrás o fluxo de atualizações da linguagem era mais lento, ocorrendo por volta de a cada 2 anos; no entanto, atualmente, o fluxo ocorre de 6 em 6 meses. Do livro que eu estou lendo, a versão mais recente é a JDK 11 de 2018, já hodiernamente 2023 já estamos na versão JDK 21, adicionando-se diversas funcionalidades atualizadas para a querida linguagem Java.

## Servlets

Dada a importância do Java no processo cliente-servidor da Internet, não era de se demorar o Java também ter o seu impacto no lado do servidor. Isto foi através dos Servlets, pequenos programas executados no servidor para se comunicar com o cliente. 
Um exemplo de seu uso é em uma loja e-commerce que planeja visualizar o preço de seus produtos em catálogo, exibindo-se os dados do banco de dados a partir de uma página web. São importantes portanto no back-end dos programas, sendo hoje em dia muito utilizados no mercado.

## Evolução do Java

O Java experienciou sérias mudanças ao longo de seu desenvolvimento. Muitas dessas mudanças pode-se identificar como: Expressões Lambda, Desprezo de Classes e Pacotes obsoletos, mudanças em estruturas de controle, anotações, módulos e diversas outras mudanças. A atual versão do Java é a JDK 21.

	