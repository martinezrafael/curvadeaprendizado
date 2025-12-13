# Funções Mock (Mock Functions)

As funções Mock são ferramentas que você usa em testes de software para simular o comportamento de funções reais.

**Nome Alternativo:"Spies" (Espiões)**

- Elas são chamadas de "espiões" porque permitem que vocẽ monitore (espione) o comportamento de uma função que é chamada por outro código, em vez de apenas verificar o resultado final (a saída) desse outro código.
- Exemplo: Em vez de apenas verificar se a função principal retornou o valor correto, você pode "espiar" se uma função auxiliar de envio de email foi realmente chamada, quantas vezes e com quais argumentos.

**Como Criar:**

- Você pode criar uma função mock usando um comando específico dop ambiente de teste(como o jest): `jest.fn()`

**Comportamento Padrão**

- Se você criar uma função mock e não fornecer a ela uma implementação (ou seja, não disser o que ela deve fazer quando for chamada), ela simplesmente retornará `undefined` (indefinido) quando for invocada.

**Em resumo**

Uma função Mock é um substituto falso de uma função real que permite que você:

1. Monitore como e quando ela é usada.
2. Controle o que ela retorna (se necessário) para isolar o código que você está testando.

**Exemplo Prático:**
Imagine que você está desenvolvendo um aplicativo e tem uma função chamada `processarPedido(pedido)`

Essa função tem duas responsabilidades:

1. Calcular o total do pedido.
2. Chamar um serviço externo para enviar um email de confirmação ao cliente.

**Cenário sem Mock**
Se você testar a função `processarPedido` no mundo real, seu teste:

- Dependerá da conexão de rede;
- Enviar um email real e cada vez que o testeforexecutado (o que é lento, caro e pode lotar a caixa de entrada do cliente de teste).

**Cenário com Mock**
Usando uma Mock Function (ou Spy) para o serviço de email, o processo fica assim:

1. Criação do Mock: Você substitui o serviço de email real por um "espião" (uma função mock);

2.Execução: Vocẽ chama `processarPedido(pedido)`

3. Teste (Espionagem): O teste não importa se o email foi enviado de verdade. Ele apenas verifica, usando o mock, se:

- O espião (`enviarEmailMock`) foi chamado (garantindo que a função não esqueceu de enviar o email);
- O espião foi chamado exatamente uma vez;
- O espião foi chamado com os argumentos corretos (por exemplo, o email do cliente e o resumo do pedido).

**Resultado:** O testeé rápidp, confiável (mão depende da internet ou de um servidor de email) e verifica o comportamento interno da função principal sem efeitos colaterais.

## Informação Adicional (Typescript e Jest)

Essa nota é uma orientação importante para quem está usando Typescript (uma linguagem que adiciona tipagem ao JavaScript) em conjunto com o framework de testes Jest.

**O que isso significa?**

- Importação Explícita: Para que os exemplos de Typescript funcionem corretamente,você precisa importar explicitamente as APIS (funções e objetos) do Jestque você for utilizar.

**Exemplo da Importação:**
`import {expect, jest, test} from '@jest/globals';`

- Isto garante que o Typescript saiba exatamente o que são `expect`, `jest` (que usamos para `jest.fn()`). e `test`.
- Guia "Getting Started": Se você tiver problemas ou precisar configurar o ambiente Jest para funcionar bem com o Typescript, a documentação recomenda consultar o guia de Primeiros Passos (Getting Started Guide) para obter instruções detalhadas de configuração.


**Referência de Propriedades da Mock Function**

`mockFn.getMockName()`
- **Tradução:** Retorna a string (o texto) do nome de mock que foi definido ao chamar o método `.mockName()`
- **Para que serve:** É útil para tornar as mensagens de erro nos seus testes mais claras. Se o seu teste falhar, saber o nome específico do mock (ex: "Serviço de Envio de Email Mock") ajuda a identificar rapidamente qual função está causando o problema.

