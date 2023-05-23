# Aprendendo o básico de Assembly


> Esse será um projeto pessoal meu onde, no qual vou me arriscar a quebrar a cabeça com essa linguagem que é um bicho de 7 cabeças. -"Por que fazer isso? essa linguagem é terrível" engenharia reversa é a resposta, quero entender o computador de dentro para fora.

[Assembly Quick Guide](https://www.tutorialspoint.com/assembly_programming/assembly_quick_guide.htm)



## Difrença entre assembly e as linguagens atuais

### Diferentes níveis de linguagem

Já que a **linguagem de máquina é basicamente composta de 0s e 1s**, e para um humano é praticamente impossível desenvolver alguma coisa dessaforma, é necessário que haja algum intermediador entre o processador da máquina e nós, e é assim que surgem as linguagens de programação. A grosso modo, as linguagens de programação seriam um conjunto de instruções e regras que utilizamos para resolver um problema, ou melhor para colocarmos o computador para resolver.

1. Linguagem de máquina
2. Linguagem hexadecimal
3. Linguagem assembly
4. Linguagem C (por exemplo)

Essa linguagem hexadecimal foi possivelmente a primeira tentativa de linguagem de programação, onde se utilizava a notação hexadecimal para representar os programas, mas a programação e leitura desses códigos continuou impraticável.

Com o desaparecimento da linguagem hexadecimal surge a linguagem de montagem: assembly, que trouxe muita praticidade para contruir coisas com os computadores utilizando suas instruções mnemônicas (exemplo: MOV abreviação para Move, que é responsável por mover valores).

Conforme as tecnologias foram avançando, linguagens como C e Pascal surgiram e trouxeram consigo o termo linguagem de "alto nível" que
saem da proposta do assembly e trazem os interpretadores e compiladores para serem os intermediários na comunicação do computador com o programador.

> Mnemônico: seriam os nomes atribuídos as funções em programas de computadores.

### Assembly e C++

Basicamente a diferença crucial entre a linguagem montada e as linguagens modernas seria que, com  assembly as instruções são traduzidas em linguagem de máquina (0s e 1s), sendo assim é necessário ter um bom conhecimento acerca do processador que se está utilizando, caso contrário, não será possível utilizar o programa se o processador não for potente o suficiente para interpretar as funções. Em linguagens como C++há um compilador que vem cheio de instruções predefinidas para faciliar para o programador e ainda assim possibilitar que o processador compile as instruções.



## Introdução

### Recursos básicos do hardware do Pc

#### Processador

O processador ou CPU é o componente que comanda tudo no computador, desde a ordem de execução de programas até o cálculo dos dados/bits. É composta por:

- **1 UC (Unidade de Controle)** que é responsável, obviamente,  por controlar e garantir que todos os componentes e dados que circulam no computador executem suas devidas funções;  

- **2 ULA (Unidade Lógica Aritmética)** todas as operações lógicas (and, or, not, etc) e aritméticas (subtração, adição, etc) são comandadas poresse compartimento;

- **3 Registradores** fornece dados da memória para o processador, __mais detalhes abaixo__.

#### Registradores

Ou registros, são um tipo de memória que está integrada a CPU em que são armazenadas as intruções referente ao funciocionamento do computador.
Há vários tipos de registros, cada um com a sua funcionalidade, exemplos: o que aponta a próxima instrução a ser executada, o que armazena dados, enfim.
Pense no processador como o rei os e vários registradores como os seus conselheiros.

#### Memória

A memória do computador é basicamente um circuito eletrônico com capacidade de armazenar dados.

##### Memória principal

Se trata de uma memória muito veloz para READ e WRITE (leitura e escrita de dados) mas sendo muito rápida ela também é vólatil, ou seja, se o computador for desligado toda a atividade que estava sendo feita será perdida. A memória que é encontrada nos PCs é a RAM (Randon Access Memory) que acessa as informações devidas de forma direta e sem que seja necessário leitura de todas as áreas desse conjunto de dados.

###### Memória de leitura 

Nesse tipo de memória  as configurações são de fábrica, logo não podem ser alteradas, a única coisa que pode ser feita é a leitura/utilização dos dados. ROM (Read Only Memory ou memória somente para leitura) é onde a BIOS (Basic Inpu/Output System) dos computadores está armazenada.

Dentre as ROMs há vários tipos:

- **1 PROM (Programmable Read Only Memory ou Memória Programável Exclusiva para Leitura)** = pode ser programada através de um equipamento específico e gravada uma única vez;

- **2 EPROM (Electrically Programmable Read Only Memory ou Memória Exclusiva para Leitura Programável Eletricamente) ou (Eraseble Programmable Read Only Memory ou Memória Exclusiva para Leitura,Programável e Apagável)** = pode ser gravada, apagada e regravada, por equipamento espacífico;

- **3 EAROM (Electrically Alterable Read Only Memory ou Memória Alterável Eletricamente)** = seus dados podem ser alterados; 

- **4 EEROM (Electrical Eraseble Programmable Read Only Memory)** = seu conteúdo pode ser apagado através de processos elétricos.

###### Memória de cache

É uma memória muito mais rápida que a RAM mas que é consideravelmente menor, sua função é armazenar temporariamente dados sem precisar buscar na memória pricipal. 

##### Memória secundária

Esse tipo de memória não tem acesso direto a CPU, mas em compensação tem a capacidade de armazenar grandes quantias de dados e de fazer a transferência segura desses dados. Exemplos comuns são: pendrives, HDs, CDs, disquetes, etc.

#### Sistema binário



# Referências

## Sites

[Difereça entre Assembly e C++](https://www.trabalhosfeitos.com/ensaios/Diferen%C3%A7a-Entre-Assembly-e-c/43443241.html)

[Níveis das linguagens de programação](http://professores.dcc.ufla.br/~monserrat/icc/Capitulo3.html)

[O que é um mnemônico? - o que é techopedia](https://pt.theastrologypage.com/mnemonic)

[Arquitetura dos computadores](http://professores.dcc.ufla.br/~monserrat/icc/Capitulo2.html)

[Memória](http://www.inf.ufsc.br/~j.barreto/cca/perifer/memorias.html)

[O que são bits, bytes, megabits, megabytes e afins?](https://www.infowester.com/bit.php)

## Imagens

[Decimal, binário e hexadecimal](https://lh4.googleusercontent.com/xSZO9mpOS7gk6VjUXklM4WIYz7FwyAk0HvwtwSXiGyP__qHQuxthodh32bLpIthg8NoUPggiDceBMdw5ORZ_hHsDhBx_5q2Ld0vaCt9AO3ByUiEsTX6IMN4vxQozXkkVKWCHDpc=s0)

[Relação do processador com a memória](http://tics.ifsul.edu.br/matriz/conteudo/disciplinas/aoc/ub/img/B1.jpg)


