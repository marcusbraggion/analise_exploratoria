![logo](https://user-images.githubusercontent.com/97288194/152074062-f2e33e2b-f28e-4061-8548-68fb7b822546.jpg)

# House Rocket

O objetivo do projeto é recomendar soluções para o negócio através de Insights gerados por uma Análise Exploratória de Dados. O projeto abrange 5 etapas do roteiro de solução de problemas da Ciência de Dados, que são: A Questão do Negócio, Compreensão do Negócio, Limpeza de Dados e Exploração de Dados.
git
# 1.0 Contexto do Negócio (fictício)

A House Rocket é uma plataforma digital cujo modelo de negócio é a compra e venda de imóveis utilizando tecnologia.
Sua principal estratégia é comprar boas casas em ótimas localizações a preços baixos e depois revendê-las a preços mais altos. Quanto maior a diferença entre comprar e vender, maior o lucro da empresa e, portanto, maior sua receita.

# 2.0 Desafio

Você é um Cientista de Dados contratado pela empresa para ajudá-lo a encontrar as melhores oportunidades de negócios no mercado imobiliário. O CEO da House Rocket gostaria de maximizar a receita da empresa encontrando boas oportunidades de negócios.

# 3.0 Premissa de Negócios

date: Dados de vendas

price: Preço de venda

rooms: Número de quartos

bathrooms: Número de banheiros

sqft_living: Tamanho da área de estar em m²

sqft_lot: tamanho do lote em m²

floors:número de pisos

Waterfront: '1' se a propriedade estiver à beira-mar, '0' se não for.

view: Um índice de 0 a 4 de quão boa é a vista do imóvel (imagine 0 para um imóvel com vista para um beco sujo e 4 para um imóvel com vista para um belo parque)
condição: estado da casa, com valores de 1 a 5

grade: Classificação pela qualidade do material da casa. Edifícios com melhores materiais costumam custar mais

sqft_above: m² acima do solo

sqft_basement: m² abaixo do solo

yr_built: yr_built: ano de construção

yrrenovated: ano de_renovado. '0' se nunca melhorou

Zip Code:CEP de 5 dígitos

lat, long: latitude e longitude

squft_livng15: tamanho médio das 15 casas mais próximas, em m²

sqft_lot15: tamanho médio do lote das 15 casas mais próximas, em m²


# 4.0 Estratégia de Solução

A estratégia adotada foi a seguinte:

Etapa 01. Descrição dos dados: Pesquisei os NAs, verifiquei os tipos de dados (e adaptei alguns deles para análise) e apresentei uma descrição estatística.

Etapa 02. Engenharia de Funcionalidades: Novas funcionalidades foram criadas para possibilitar uma análise mais completa.

Etapa 03. Análise Exploratória de Dados: Realizei análises de dados univariados, bivariados e multivariados, obtendo propriedades estatísticas de cada um deles, correlações e testando hipóteses (as mais importantes estão detalhadas na seção a seguir).

Passo 04. Interpretar e Traduzir para o negócio: O desempenho da análise é convertido em valores de negócio.

# 5.0 Top 3 Insights

## **H1**. Preços dos imóveis aumentam mais com o número de andares ao números de banheiros
**VERDADEIRA** Números de banheiros impactam mais o valor ao número de andares

## **H2**. Preços dos imóveis aumentam mais com o tamanho do porão ao números de andares.
**VERDADEIRA** O tamanho do porão influencia mais o aumento de preço ao número de andares.

## H3. Preços dos imóveis aumentam mais quando possuem vista para o mar ao número de banheiros no imóvel.
**VERDADEIRA** O atributo ''vista para o mar'' impacta mais no preço ao número de banheiros do imóvel.

# 6.0 Conclusão

Encontramos uma oportunidade de negócio ao localizar imóveis com preços abaixo da mediana local. Então identifiquei que a sazonalidade influencia no preço, a temporada de primavera tende a encarecer o imóvel, então a temporada de verão. Então sugeri um aumento de 0,30% no preço de compra quando for primavera e 0,20% quando for verão e 10% no restante dos imóveis que não se enquadram nesses cenários.
Por fim, foi possível identificar oportunidades de negócios que resultaram em um lucro total de R$ 15.981.245,72.

# 7.0 Próximos passos

Desenvolver um mapa interativo com geolocalização de cada propriedade de id por uma API.

Desenvolver um modelo de aprendizado de máquina para prever o valor de revenda correto das propriedades e identificar oportunidades que não podemos alcançar por meio da análise de dados.
