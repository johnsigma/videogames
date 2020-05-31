# Uma pequena análise sobre venda de jogos de videogames

Pequena análise de dados sobre venda de jogos de videogames, feita apenas como um projeto pessoal de análise de dados, o conjunto de dados foi obtido através do link: https://www.kaggle.com/gregorut/videogamesales/data. Lá se encontra também a descrição de cada campo do dataset. Importante ressaltar que esse dataset é constituído apenas por jogos que venderam ao menos 100000 cópias e não considera as plataformas do PC como Steam, GOG, etc.
Para essa análise eu usei a linguagem Python e algumas bibliotecas para análise de dados como o Pandas.

O dataset fornecido está em formato CSV e está em ordem decrescente pelo número de vendas globais (em milhões de cópias).

*Vamos exibir os 5 jogos mais vendidos no mundo todo:*

```python
# importando os pacotes
import pandas as pd
# lendo o arquivo
df = pd.read_csv("/content/vgsales.csv")
# exibindo os 5 primeiros resultados
df.head()

```

