# javascript-atividade-dividir-conta

# Entrega: Dividindo o Valor das Compras

## Descrição

Neste exercício, você irá implementar um código que calcula o valor total das compras e decide como dividir o custo entre duas pessoas. Dependendo se o valor total é par ou ímpar, a lógica de divisão será diferente.

## Objetivo

- Calcular o valor total de uma lista de itens, considerando a quantidade de cada item.
- Determinar como dividir o custo total entre duas pessoas com base em uma regra de paridade do valor.

## Lógica do Exercício

O exercício está dividido em duas partes principais:

1. **Cálculo Inicial com Quantidades Fixas**
   - A primeira parte do código calcula o valor total de uma lista fixa de produtos, com quantidades já definidas.
   - Caso o valor total das compras seja **par**, uma pessoa paga o vinho e o valor sem o vinho é dividido igualmente entre as duas pessoas.
   - Caso o valor total seja **ímpar**, o valor total é dividido igualmente entre as duas pessoas.

2. **Cálculo com Quantidades Informadas pelo Usuário**
   - A segunda parte do código solicita ao usuário a quantidade de cada item através de prompts.
   - Calcula o valor total com as quantidades informadas.
   - A divisão do valor segue a mesma regra de paridade da primeira parte.

## Produtos e Preços

Os seguintes produtos e seus respectivos preços são considerados no cálculo:

- **Refrigerante**: R$12
- **Macarrão**: R$7
- **Ervilha**: R$7
- **Arroz**: R$23
- **Feijão**: R$12
- **Vinho**: R$70

## Detalhes da Implementação

### Variáveis Utilizadas

- **Preços Fixos dos Produtos**: São armazenados em variáveis como `refrigerantePreco`, `macarraoPreco`, etc.
- **Quantidade de Itens Fixos**: Variáveis como `valorTotalRefri`, `valorTotalMacarrao`, etc., calculam o valor total com base nas quantidades fixas.
- **Total Geral**: Variável `total` calcula o valor total de todos os itens.
- **Total sem Vinho**: Variável `totalSemVinho` calcula o valor total excluindo o vinho, para possibilitar a divisão do valor em caso de paridade.

### Fluxo de Controle

- **Cálculo Inicial**: Após calcular o valor total, um `if` verifica se o valor é par (`total % 2 == 0`).
  - Se **par**: O vinho é pago por uma pessoa, e o restante é dividido.
  - Se **ímpar**: O valor total é dividido igualmente.

- **Interação com o Usuário**: Através de `prompt()`, o usuário informa a quantidade de cada produto desejada. Novos valores totais são calculados e o mesmo processo de verificação de paridade é aplicado.

### Exemplo de Saída

- **Console Log** ou **Alert**:
  - Caso o valor seja **par**:
    ```
    O valor total foi par, você paga o vinho sozinho, fica X para mim, e o restante para você.
    ```
  - Caso o valor seja **ímpar**:
    ```
    O valor total deu ímpar, vamos dividir tudo, Y para cada um.
    ```

## Dicas

- Utilize o operador `%` (módulo) para verificar se o valor é par ou ímpar.
- Para calcular o valor total, multiplique o preço pela quantidade desejada de cada item.
- Use `prompt()` para solicitar informações do usuário e `alert()` para exibir o resultado.

## Contribuições

- Se você encontrar algum problema ou tiver sugestões para melhorar o código, sinta-se à vontade para abrir uma _issue_ ou enviar um _pull request_.

## Licença

- Este repositório está sob a licença MIT. Veja o arquivo `LICENSE` para mais detalhes.

