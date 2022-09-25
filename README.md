![Logo_project](https://github.com/Matheus2510/Atualiza_Sheets_Periodicamente/blob/main/folder/sheets_python.png)

# Atualização de Base de Dados - Google Sheets

Trata-se de uma maneira de atualizar uma base atualizada periodicamente que, em sua estrutura, tem indicado o próprio período. Exemplo: uma tabela atualizada diariamente, que possui uma de suas colunas indicando a data; ou uma tabela atualizada mensalmente, com uma de suas colunas indicando o mês.

O objetivo é evitar a duplicação de dados caso seja necessário complementar ou mesmo revisar determinado período. Exemplo: pagamentos de boletos podem compensar no dia seguinte ou em até 3 dias úteis após o pagamento em si. Em todo caso, se o que importa é a data de pagamento, é necessário atualizar a base de dados de um certo período pelo menos algumas vezes, e corre-se o risco de repetir informações que já estavam na base de dados.

## Tecnologias

* Python versão 3.7.14
* Arquivos em formatos diversos (csv, xlsx, json, etc)

## Serviços utilizados

* Google Colab
* Google Drive
* Google Sheets

## Como usar

Inicialmente, é preciso executar o primeiro trecho do código (Imports) para que suas credenciais sejam identificadas e o Google Colab tenha acesso ao seu Google Drive.

Em seguida, a partir dos arquivos/fontes brutos de onde os dados úteis serão extraídos, realiza-se a tratativa destes mesmos dados a fim de deixá-los no formato e estrutura do destino final, sempre somente com um período de cada vez.

Com o dataframe resultante em mãos, basta executar a função *atualiza_sheets* com os seus cinco parâmetros: sheet (nome da planilha a ser atualizada), worksheet (nome da aba a ser atualizada), df (dataframe final), coluna_periodo (nome da coluna que indica a granularidade dos dados) e período_str (o período específico que está sendo atualizado, como a data).

No arquivo do código, foram criados dados fictícios para os dias 01/08/2022, 02/08/2022 e 03/08/2022. Alguns dos dados do dia 01 já constam na sheets de exemplo.

Após a execução do laço for, os dados dos 3 períodos de exemplo serão atualizados.

![sheet_pre_atualizacao](https://github.com/Matheus2510/Atualiza_Sheets_Periodicamente/blob/main/folder/Sheets.png)

## Features

* Automatização de atualização de relatórios
* Manipulação de sheets com python

## Versão

* 1.0.0.0

## Autores

* Matheus Henrique de Souza: @Matheus2510 (https://github.com/Matheus2510)
