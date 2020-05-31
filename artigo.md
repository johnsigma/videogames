# Uma pequena análise sobre venda de jogos de videogames

Pequena análise de dados sobre venda de jogos de videogames, feita apenas como um projeto pessoal de análise de dados, o conjunto de dados foi obtido através do link: https://www.kaggle.com/gregorut/videogamesales/data. Lá se encontra também a descrição de cada campo do dataset.

Para essa análise eu usei a linguagem Python e algumas bibliotecas para análise de dados como o Pandas.

Importante ressaltar que os jogos são separados por plataformas, então um mesmo jogo será listado mais de uma vez se ele foi comercializado em mais de uma palataforma.

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

![Alt text](https://github.com/johnsigma/videogames/blob/master/imagens/saida01.png "5 jogos mais vendidos dos videogames")

Nesta imagem percebemos que o dataset possui 11 colunas, a seguir listarei as colunas e detalharei o que elas representam:
* Rank = Classificação, nesse caso a os jogos estão classificados em ordem decrescente pelo número de vendas global (Global_Sales)
* Name = Nome do jogo
* Platform = Plataforma onde o game foi avaliado, nesse caso são os consoles
* Year = Ano de lançamento do jogo
* Genre = Gênero do jogo
* NA_Sales = Vendas na América do Norte
* EU_Sales = Vendas na União Europeia
* JP_Sales = Vendas no Japão
* Other_Sales = Vendas no resto do mundo
* Global_Sales = Vendas no mundo todo

Utilizando o comando .shape[0] obtemos o número de linhas desse dataset, nesse caso quantos jogos foram considerados:

![Alt text](https://github.com/johnsigma/videogames/blob/master/imagens/saida02.png "Número de jogos considerados")

Então temos que 16598 jogos foram considerados nesse levantamendo de dados.

Vamos agora verificar quais plataformas foram consideradas:
![Alt text](https://github.com/johnsigma/videogames/blob/master/imagens/saida03.png "Plataformas")


