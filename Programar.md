## O que é programar?

**Antes dos Computadores**

- Antes dos computadores nós tinhamos: problemas reais com soluções repetidas;
- O conceito de **programar** é basicamente descrever uma **sequência de passos** (receitas, rotinas);

**Primeiros Computadores**

- Com os primeiros computadores, era possível passar **instruções** para ele **de forma detalhada**;
- Os comptadores só sabem fazer o que a gente manda;
- Nos primórdios da programação, a forma como a gente pedia ou ensinava coisas para o computador, era através de **cartões perfurados**;

```
Programar é dar instruções detalhadas para uma máquina executar uma tarefa.
```

A tecnologia muda:
**Evolução da arte de escrever código**

- Começamos, **falando do cartão perfurado**, que era uma das formas que tinhamos de **introduzir dados** para um computador (anos 1940 - 1960);
- Com o passar do tempo, as coisas foram evoluindo e então chegamos no **Assembler & Código de Máquina (baixo nível)**
- As instruções Assembler, são **instruções simples e direta** para o hardware;
- Mas são pouco "humano", muito detalhado.

**Linguagens de alto nível** -> Mais próximo do ser humano

- Com uma linguagem de lto nível, programar passou a ser: usar comandos mais próximos da nossa linguagem;
- Com isso, a gente faz com que aprender uma linguagem de programação se torne mais fácil, então damos mais poder para as pessoas.

**Programação estruturada e orientada a objetos**

- O objetivo era ter programas mais organizados;
- A ideia do objeto é ter representações do mundo real, dentro do nosso código.

**Low-Code/No-Code**

- Programar sem escrever código;
- Arrastar e soltar para criar aplicações;

**Prompt Engineering**

- Programar conversando com a IA;
- Escrever comandos/desafios para modelos como o ChatGpt.

## Para saber mais: da linguagem aos bits

**O Universo Binário**

Embora à primeira vista o mundo dos algoritmos pareça distante dos 0 e 1, a realidade é que cada instrução escrita e uma linguagem de programação precisa ser eventualmente conversada em uma linguagem que o computador compreenda: o binário. Esse sistema númerico, baseado em apenas dois digítos - 0 e 1 - é a forma na qual os dados e comandos são codificados no hardware. Essa conversão é essencial para que ocorram todas as operações, desde cálculos simples até o gerenciamento de sitemas complexos.

**Do código ao Código de Máquina**

Quando um programador escreve um código em uma linguagem de alto nível, como JavaScript, esse código ainda está em uma forma abstrata e legível para nós. É o trabalho dos compiladores e interpretadores que convertem essas instruções para uma linguagem de máquina. Essa tradução pode ocorrer em tempo de execução (como acontece em linguagens interpretadas) ou previamente, gerando um arquivo executável. Em ambos os casos, o resultado final consiste em um fluxo de comandos em binário, que aciona operações fisícas nos circuitadores do processador.

**Por que a conversão é necessária?**

A razão pela qual os computadores operam somente com 0s e 1s está intrinsicamente ligada à sua arquitetura física. Os transistores, que formam a base dos circuitos eletrônicos, possuem estados ligados e desligados, correspondendo naturalmente aos valores binários. Essa simplicidade não só torna o design de circuitos mais confiável, mas também facilita a detecção de erros e a implementação de mecânismos de redundância para garantir a integridade dos dados.

**Abordagens na Tradução do Código**

Um aspecto interessante é diferenciar os processos de **compilação** e **interpretação**:

- em ambientes compilados, o código inteiro é traduzido para linguagem de máquina antes de ser executado, proporcionando melhor performance, uma vez que a tradução já ocorreu integralmente.

- Em ambientes interpretados, a conversão acontece enquanto o programa é executado, o que permite maior flexibilidade e portabilidade, mas pode resultar em execuções ligeiramente mais lentas.

Cada abordagem tem suas vantagens e desvantagens, impactando tanto a velocidade de execução quanto a facilidade de desenvolvimento e adaptação a diferentes plataformas.

Esse entendimento acerca da jornada do código - da linguagem escrita até os sinais binários que comandam o hardware - é fundamental para compreender a profundidade e a complexidade que estão por trás do ato de programar.

## Para saber mais: bibliotecas e frameworks

Quando começamos a aprender programação e desenvolvimento de software, é comum encontrarmos termos como framework e biblioteca. Ambas são ferramentas que ajudam pessoas desenvolvedoras a escrever menos código e resolver problemas de forma mais rápida, mas funcionam de maneiras diferentes. Vamos entender melhor cada uma delas, a seguir.

**Biblioteca: uma coleção de ferramentas úteis**

Uma biblioteca é como uma caixa de ferramentas com funções especifícas já prontas que você pode usar no seu código para não ter que escrever tudo do zero.

Por exemplo, se você precisa fazer um cálculo complicado ou mostrar uma animação, em vez de criar tudo do início, pode usar uma biblioteca que já tem essa função pronta. Você escolhe quando e como usar essas ferramentas no seu código.

```
Um ótimo exemplo de biblioteca é a jQuery, mencionada anteriormente em vídeo, que facilita a
manipulação de elementos de uma página HTML, sem que você precise escrever comandos complexos.
```

**Framework: uma estrutura para seguir**

Um framework é uma estrutura pronta que ajuda você a construir um projeto de forma mais organizada e eficiente. Ele já vem com várias regras, funções e caminhos definidos - como se fosse um molde ou uma base para começar a construir.

A principal diferença em relação a uma biblioteca é o controle do fluxo: com uma biblioteca, você chama o que quiser, quando quiser. Com um framework, é ele quem chama partes do seu código no momento certo. Ou seja, você encaixa seu código dentro do que o framework já espera - isso é conhecido como inversão de controle.

Pense em um framework como um kit de montar móveis com manual: ele já traz as peças, o passo a passo e até algumas ferramentas. Você segue o plano e monta o móvel mais rápido, com menos chances de erro. E sim, um framework pode conter várias bibliotecas - e isso é bastante comum!

```
Um exemplo de framework é o Angular (usado para criar aplicações web). Ele já vem com: uma biblioteca
para lidar com formulários, outra para fazer requisições HTTP, outra para trabalhar com rotas (endereços da aplicação) e muito mais...
```

**Por que usar essas tecnologias?**

Bibliotecas e frameworks existem para economizar tempo, evitar erros comuns e seguir boas práticas. Em vez de reinventar a roda, você usa soluções que já foram testadas por milhares de pessoas desenvolvedoras. Com o tempo, aprender a escolher e usar essas ferramentas se torna parte do seu crescimento como dev.
