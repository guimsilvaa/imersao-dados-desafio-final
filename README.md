# Modelos de machine learning para predizer o potencial de fármacos para atuar no sistema nervoso central 
Projeto apresentado como desafio final do curso Imersão de Dados - 3ª Edição - ALURA, sob a temática Data Science & Drug Discovery 
<br />
![imagem mostrando no canto superior direito a opção Fork](https://github.com/guimsilvaa/imersao-dados-desafio-final/blob/main/Dados/ga.jpg?raw=true)

# Background do projeto #
O planejamento racional e descoberta de fármacos (do inglês "drug design & discovery") é um processo caro e demorado, levando de 10-20 anos e custando bilhões de dólares [1](https://link.springer.com/article/10.1007/s00210-016-1216-8). Nas etapas iniciais deste processo é imprescíndivel fazer o uso de técnicas computacionais que permitam guiar e predizer as propriedades desejáveis para um candidato a fármaco (composto químico) sob estudo [2](https://link.springer.com/article/10.1007/s10822-016-9993-1). 

*Drug-likeness* é um termo - tradução literal do inglês "fármaco-similar" - usado, de modo geral, para indicar o quão similar é determinado composto químico à fármacos já conhecidos [3](https://onlinelibrary.wiley.com/doi/abs/10.1002/3527603743.ch17). Tal similaridade é avaliada em termos de propriedades físico-químicas e características estruturais (chamados descritores), e pressupõe-se da ideia de que quanto mais parecido, maior a chance de determinado composto vir a se tornar um fármaco [4](https://doi.org/10.3797/scipharm.0802-05).

Para se predizer a *drug-likeness* de compostos, existem diversas abordagens que vão desde simples regras/critérios até o uso de modelos matemáticos e estatísticos preditivos e mais complexos. Neste contexto, considerando o grande número de dados disponíveis atualmente, principalmente de diferentes descritores, o uso de machine learning torna-se bastante relevante [5](https://doi.org/10.3389/fchem.2018.00162). 

# Objetivos #
Neste projeto, busquei desenvolver modelos de machine learning com vista à predição do potencial de novos compostos virem a ser fármacos que atuem no sistema nervoso central (SNC), ou seja, candidatos a fármacos para doenças neurodegenerativas e demais disturbios psiquiátricos, tais como doença de Alzheimer, Parkinson, depressão, ansiedade, dentre outras.

# Dados utilizados #
Para isso foi usado uma série de 1150 compostos previamente classificados como drogas do SNC (ou CNS drugs) e drogas sem habilidade de atuar no SNC (non-CNS drugs), extraídas da literatura [6](http://dx.doi.org/10.1021/acs.jmedchem.8b01388). Calculou-se os descritores químicos destes compostos usando o nodo RDKit implementado no Knime [7](http://www.rdkit.org) e foram usadas as seguintes técnicas de machine learning: regressão logística, árvore de decisão e *random forest*. Todos os modelos foram validadios com respeito as respectivas acurácias, a partir do uso de séries de treinamento e teste, bem como comparando-se com um modelo ingênuo que fora gerado.

# Highlights e conclusões #
* Uso de dataset com mais de mil fármacos separados em ativos e não-ativos no SNC.
* Comparação e análise de histogramas e boxplots de descritores fundamentais.
* 3 modelos de machine learning apresentando acurácias acima de 80%.
* Destaque para o modelo de random forest com 87% de acurácia. 
* Demais refinamentos deverão ser feitos considerando-se as boas práticas de modelagem.

# Referências e links #
- [1] https://link.springer.com/article/10.1007/s00210-016-1216-8
- [2] https://link.springer.com/article/10.1007/s10822-016-9993-1
- [3] https://onlinelibrary.wiley.com/doi/abs/10.1002/3527603743.ch17
- [4] https://doi.org/10.3797/scipharm.0802-05
- [5] https://doi.org/10.3389/fchem.2018.00162
- [6] http://dx.doi.org/10.1021/acs.jmedchem.8b01388
- [7] RDKit: Open-source cheminformatics. http://www.rdkit.org


> Author: Guilherme M. Silva (silvagm@usp.br)
> <br />PhD student from the Computational Laboratory of Pharmaceutical Chemistry (LCQF), at the FCFRP - USP Ribeirão Preto, Brazil
