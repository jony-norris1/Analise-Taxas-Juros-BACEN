# Análise de Taxas de Juros do Banco Central

Este repositório contém código em Python para coletar, analisar e visualizar séries temporais das taxas de juros do Banco Central, incluindo Selic e CDI.

## Fonte de Dados

Os dados são obtidos por meio de web scraping do site do Banco Central:

Por favor, conclua esta parte do código:

```python
import requests
from bs4 import BeautifulSoup

url = "https://www3.bcb.gov.br/sgspub/consultarvalores/consultarValoresSeries.do?method=getPagina"
response = requests.get(url)
soup = BeautifulSoup(response.text, 'html.parser')
```
# Dados Coletados

Os dados são salvos localmente em:

- dadosbacen.csv

Com as seguintes características:

- Delimitador: ponto e vírgula (;)
- Encoding: UTF-8
- Colunas:
  - Data
  - Selic
  - CDI
  - Outras taxas

# Análise e Visualização

O dataframe é analisado utilizando Pandas, incluindo:

- Limpeza e tratamento dos dados
- Análise estatística descritiva
- Visualizações com Matplotlib e Seaborn

  ## Notebook de Análise

O código completo de análise pode ser visto neste Colab:

**https://colab.research.google.com/drive/1WQuR2T3mAOIi5-TLrW0ACrf8Gd9DKuew**


