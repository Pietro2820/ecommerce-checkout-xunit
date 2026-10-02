# Ecommerce Checkout xUnit

Solução .NET 10 para gerenciar o cálculo de cupons, itens e frete de uma loja online, com testes unitários utilizando xUnit.

## Métodos Implementados

1. `GerarCodigoRastreio(string regiao, int numeroPedido)`: Gera um código de rastreio formatado com a região em maiúsculas e o número do pedido com 4 dígitos.
2. `CalcularPontosFidelidade(int valorTotal)`: Calcula os pontos de fidelidade (2 pontos para cada R$ 10 em compras).
3. `TemDireitoAFreteGratis(int valorTotal, bool eClienteVIP)`: Verifica se o cliente tem direito a frete grátis (valor >= 200 ou cliente VIP).

## Cobertura de Testes

- Teste de formatação de string (`Assert.Equal`).
- Teste de cálculo numérico (`Assert.Equal`).
- Testes de lógica booleana para frete grátis (`Assert.True` e `Assert.False`).

## Instruções de Execução

1. Clone o repositório.
2. Navegue até a pasta da solução no terminal.
3. Restaure as dependências:
   ```bash
   dotnet restore