# README

## Visão Geral

Este script em Python obtém dados de mortalidade do [Ministério da Saúde do Brasil](https://svs.aids.gov.br/) usando a API deles. Os dados são filtrados com base em parâmetros específicos, processados e analisados. O script gera um arquivo CSV contendo informações de mortalidade para o ano de 2020 e cria um gráfico de barras horizontal ilustrando a porcentagem de mortes por capítulos da CID-10.

## Requisitos

Certifique-se de ter as bibliotecas Python necessárias instaladas. Você pode instalá-las usando o seguinte comando:

```bash
pip install icd10-cm pandas requests matplotlib
```

## Uso

1. Execute o script em um ambiente Python.
2. O script utiliza a função `getDataFromSIM` para obter dados de mortalidade da API. Ajuste os parâmetros dentro da chamada da função para personalizar a recuperação de dados.
3. O script faz o download dos dados de mortalidade para o ano de 2020, os processa e gera um arquivo CSV chamado `morte_todos_todos.csv`, personalize o nome conforme os parâmetros que você utilizar
4. O script também faz o upload de um arquivo CSV para análise adicional. Siga as instruções para selecionar o arquivo apropriado.
5. Uma vez carregados, os dados são combinados e analisados, resultando em uma ordenação por ordem decrescente de mortes.
6. O script cria um gráfico de barras horizontal mostrando a porcentagem de mortes por capítulo da CID-10 no ano de 2020 para todas as faixas etárias. O gráfico é exibido e pode ser salvo conforme necessário.
