# Metodologia para Cálculo do Índice Conectar

![imagem](https://consorcioconectar.org/images/logo_conectar_fnp2.png)

Com a criação do Conectar - Consórcio Nacional de Vacinas das Cidades Brasileiras pela Frente Nacional
de Prefeitos (FNP) apresentou-se a necessidade de se elaborar um índice que orientasse a entidade na
distribuição de recursos originários de doações privadas. A partir de proposta metodológica elaborada pela
Aequus Consultoria, foi desenvolvido o Índice Conectar, conforme as diretrizes, metodologia e fórmulas
de cálculo detalhadas na [Resolução 17-2022](https://consorcioconectar.org/images/resolucao_17_2022_doacoes_privadas.pdf).

## Sobre o Índice

O Índice Conectar final varia entre 0 e 1, sendo composto por um conjunto de quatro indicadores, para os quais foram atribuídos pesos relativos na composição final do Índice. 
I - Indicador da Receita Corrente Per Capita (RC) – 50%; 
II - Indicador da Cobertura da Saúde Suplementar (CS) – 20%; 
III - Indicador da Produção Hospitalar Municipal (PH) – 15%; 
IV - Indicador da Produção Ambulatorial Municipal (PA) – 15%.

![composicao](https://github.com/vinicius-macario/indice_conectar/blob/main/indice-composicao.png)

O quanto mais próximo de um, mais confortável é a situação do município em relação aos seus pares.
O quanto mais próximo de zero, mais vulnerável é a situação do ente em relação aos seus pares.


## Notebooks

Os notebooks contém
 - Tratamento de cada fonte de dado.
 - Implementação do cálculo do Índice.
 
 
###  Fontes de dados utilizadas

#### A-Dados Populacionais

Fonte: IBGE

Descrição: Estimativas da População publicadas no DOU

https://www.ibge.gov.br/estatisticas/sociais/populacao/9103-estimativas-de-populacao.html?=&t=oque-e 

#### B-Índice de Preços ao Consumidor Amplo (IPCA)

Fonte: SIDRA/IBGE

Descrição: Tabela 1737 - IPCA - Série histórica com número-índice, variação mensal e variações acumuladas em 3 meses, em 6 meses, no ano e em 12 meses (a partir de dezembro/1979)

https://sidra.ibge.gov.br/tabela/1737

##### C-Indicador da Receita Corrente Per Capita – RC

Fonte: SICONFI/Secretaria do Tesouro Nacional

Descrição: Consulta Finbra Contas Anuais, Escopo Municípios, Tabela Receitas Orçamentárias (Anexo IC)

https://siconfi.tesouro.gov.br/siconfi/index.jsf 

##### D-Indicador da Cobertura da Saúde Suplementar – CS

Fonte: ANS TABNET/Agência Nacional de Saúde Suplementar

Descrição: Beneficiários por Município, Conteúdo Assistência Médica

http://www.ans.gov.br/anstabnet/cgi-bin/dh?dados/tabnet_02.def 

##### E-Indicador da Produção Hospitalar Municipal – PH

Fonte: DATASUS/Ministério da Saúde

Descrição: Conteúdo = Dias permanência; Esfera Jurídica = Administração Públicas Municipal

http://tabnet.datasus.gov.br/cgi/deftohtm.exe?sih/cnv/qibr.defAp%C3%B3s 

##### F-Indicador da Produção Ambulatorial – PA

Fonte: DATASUS/Ministério da Saúde

Descrição: Conteúdo = QTD. Apresentada, Esfera Jurídica = Administração pública Municipal.

http://tabnet.datasus.gov.br/cgi/deftohtm.exe?sia/cnv/qabr.def 
