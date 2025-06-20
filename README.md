# SelicBC
Desenvolver uma aplicação em C# capaz de consumir dados de uma API pública relacionada à taxa Selic, processar as informações e disponibilizar funcionalidades de consulta, exportação e cálculo.

## 🎯 Objetivos

- Consumir a seguinte API REST do Banco Central: `https://api.bcb.gov.br/dados/serie/bcdata.sgs.4390/dados?formato=json`
- Serializar os dados retornados em uma classe chamada `SelicBC`.
- Exibir um menu de navegação com opções para consulta, exportação e cálculo.
- Aplicação feita em C# com .NET 8 e com foco em boas práticas.

## 💡 Funcionalidades

- Requisição HTTP para consumo da API pública de dados Selic.
- Exportar para CSV ou Excel.
- Serialização dos dados JSON em objetos fortemente tipados.
- Exibição de menu interativo com opções para o usuário.
- Validação de entrada de dados e tratamento de exceções.
- Cálculo de juros compostos com base nas taxas Selic.
- *(Opcional)* Persistência local em banco de dados SQLite.

## ⚠️ Observações Importantes

- A aplicação deve informar claramente como o usuário deve inserir os dados.
- Trate corretamente erros de entrada de dados e falhas na comunicação com a API.
- No cálculo de juros, apresente o valor original, o valor dos juros acumulados e o valor total corrigido.

## ☁️ Exemplo de Menu

- O desenvolvedor é livre para propor um novo leiaute de menu e logica de navegação.

```
-------------------------------------------------------

                      Selic

-------------------------------------------------------              
1 - Coletar Dados da API

2 - Exportar Dados - Input: (data inicial / data final)
    2.1 - Ordenado por data mais recente
    2.2 - Ordenado por data mais antiga

3 - Exibir Dados - Input: (data inicial / data final)
    3.1 - Ordenado por data mais recente
    3.2 - Ordenado por data mais antiga

4 - Calculo de Juros - Input: (mês/ano e Valor a ser corrigido com o juros)

5 - Salvar no banco de dados sqlLite (opcional)

9 - Sair
-------------------------------------------------------
```
