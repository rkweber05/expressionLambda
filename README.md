# Expressões Lambda

## O que é uma Expressão Lambda?

Uma expressão lambda é uma função anônima que pode ser usada como argumento para passar comportamentos ou ser atribuída a variáveis. Em várias linguagens de programação, como Java, Python, e JavaScript, as expressões lambda permitem a escrita de funções concisas e com menos código.

Em termos simples, as expressões lambda ajudam a tornar o código mais conciso, especialmente quando precisamos passar pequenas funções como parâmetros ou criar funções rápidas de uma única linha.

### Estrutura Básica

A estrutura de uma expressão lambda pode ser dividida em três partes:

1. **Lista de Parâmetros**: Os parâmetros da função, que podem ou não ser explicitamente tipados, dependendo da linguagem.
2. **Operador Lambda**: Geralmente representado pela seta `->` ou `=>`, dependendo da linguagem.
3. **Corpo da Função**: O código a ser executado pela função lambda.

### Exemplo em Java

```java
// Forma tradicional de implementar uma interface funcional com uma classe anônima
Runnable r1 = new Runnable() {
    @Override
    public void run() {
        System.out.println("Executando uma tarefa.");
    }
};

// Usando expressão lambda
Runnable r2 = () -> System.out.println("Executando uma tarefa.");

## Vantagens das Expressões Lambda
1. Concisão: As expressões lambda permitem uma sintaxe mais curta, eliminando a necessidade de escrever funções anônimas completas.
2. Flexibilidade: As lambdas podem ser passadas como parâmetros para outras funções ou métodos.
3. Leitura: Em muitos casos, elas tornam o código mais legível, especialmente ao lidar com funções de alta ordem, como mapeamento, filtragem e redução.

## Quando Utilizar Expressões Lambda
As expressões lambda são úteis quando:
  * Você precisa passar uma função como argumento para um método.
  * Você deseja implementar interfaces funcionais em Java, como Comparator ou Runnable, sem ter que escrever uma classe completa.
  * Em Python e JavaScript, quando você precisa de funções rápidas e curtas, sem a necessidade de definição completa de uma função tradicional.

## Interface Funcional em Java
As expressões lambda em Java são frequentemente utilizadas com interfaces funcionais, que são interfaces com apenas um método abstrato. Um exemplo comum é a interface Comparator:
List<String> nomes = Arrays.asList("João", "Ana", "Carlos");

// Usando expressão lambda para ordenar a lista em ordem alfabética inversa
Collections.sort(nomes, (s1, s2) -> s2.compareTo(s1));

## Limitações
  * Debugging: Pode ser mais difícil depurar expressões lambda em comparação com métodos tradicionais, pois elas são anônimas e não têm um nome.
  * Legibilidade: Em situações complexas, expressões lambda podem prejudicar a legibilidade, especialmente se usadas excessivamente ou para tarefas que exigem mais de uma linha de código.

## Conclusão
  As expressões lambda são uma ferramenta poderosa para escrever código conciso e funcional em várias linguagens de programação. Elas melhoram a flexibilidade e reduzem a necessidade de classes anônimas, tornando o código mais curto e legível. Contudo, é importante utilizá-las com cuidado para evitar problemas de legibilidade e complexidade desnecessária.
