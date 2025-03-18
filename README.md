# Gerador de CPF Aleatório

Este projeto é um gerador de **CPFs** aleatórios válidos. O código utiliza um algoritmo matemático para calcular os dois últimos dígitos de um CPF, tornando o CPF gerado válido. O sistema cria **100 CPFs** válidos e os imprime no console.

## Objetivo

O objetivo deste exercício é gerar **CPFs válidos** de forma automatizada. O código cria **100 CPFs aleatórios**, calcula seus dois últimos dígitos (os chamados "dígitos verificadores") e imprime os CPFs completos no formato correto.

## Como Funciona

1. O código gera uma sequência de **9 dígitos aleatórios**.
2. Utilizando esses 9 dígitos, o código calcula o **primeiro dígito verificador** utilizando um algoritmo matemático que envolve multiplicações e divisões com uma contagem regressiva.
3. Com os 9 dígitos iniciais e o primeiro dígito verificador, o código calcula o **segundo dígito verificador** da mesma maneira.
4. O programa imprime o CPF completo no formato correto, no formato `XXX.XXX.XXX-XX`.

### Explicação do Algoritmo:
- O código gera **9 dígitos aleatórios** para o CPF.
- Ele calcula o **primeiro dígito verificador**:
  - Multiplica cada um dos 9 dígitos por um contador regressivo, somando os resultados.
  - O primeiro dígito é calculado a partir dessa soma e, em seguida, ajustado conforme a regra do CPF.
- O **segundo dígito verificador** é calculado de maneira similar ao primeiro, utilizando os 9 dígitos e o primeiro dígito verificador já calculado.

## Estrutura do Código

1. **Geração dos 9 primeiros dígitos**:
   - A função **`random.randint(0, 9)`** é utilizada para gerar os números aleatórios.
2. **Cálculo do primeiro dígito verificador**:
   - A soma dos produtos dos dígitos por um contador regressivo é usada para calcular o primeiro dígito.
3. **Cálculo do segundo dígito verificador**:
   - A soma é realizada de forma semelhante para calcular o segundo dígito.
4. **Formatação do CPF**:
   - O CPF gerado é concatenado no formato `XXX.XXX.XXX-XX`.

## Exemplo de Execução

O código gera **100 CPFs** válidos e os imprime no console. Aqui está um exemplo de saída:

```
184.562.674-82
063.449.219-05
512.043.890-00
912.027.876-80
...
```

## Como Usar

1. Clone ou baixe este repositório.
2. Abra o arquivo Python no seu editor de código favorito.
3. Execute o programa.
4. O programa irá gerar **100 CPFs válidos** e exibi-los no console.

## Requisitos

- Python 3.x

## Contribuindo

Se você deseja contribuir para este exercício, pode adicionar novas funcionalidades, como:
- Modificar o número de CPFs gerados.
- Melhorar o formato de exibição (incluir formatação com pontos e traços, como o formato tradicional de CPF).

Para contribuir:
1. Fork o repositório.
2. Crie uma nova branch.
3. Faça suas modificações.
4. Abra um **pull request** com suas alterações.

## Licença

Este projeto é de código aberto e pode ser modificado ou compartilhado conforme necessário.

---

Se tiver alguma dúvida ou sugestão, sinta-se à vontade para entrar em contato! 😄
