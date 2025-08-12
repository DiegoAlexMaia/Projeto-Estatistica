# Projeto de Estatística Aplicada

## 🧑‍💻 Autores  
- Diego Alex Maia de Lima (202411210032) - diego.maia@academico.ifpb.edu.br  
- Ivan Javier Pereira Martinez (202411210033) - ivan.javier@academico.ifpb.edu.br  
- Samuel Rodrigues Agra (202411210018) - agra.samuel@academico.iifpb.edu.br  

## 🎯 Tema e Motivação  
Neste projeto, vamos investigar a relação entre as emissões históricas de gases do efeito estufa, especialmente o dióxido de carbono (CO₂), e o crescimento econômico dos países ao longo do século XX. A ideia central é analisar se os países que mais contribuíram para o aquecimento global também foram os que mais enriqueceram, considerando indicadores como o PIB per capita e a emissão cumulativa de CO₂.

Essa análise é motivada por discussões cada vez mais frequentes sobre justiça climática e responsabilidade histórica. A crise climática atual tem impactos globais, mas as contribuições para ela são extremamente desiguais. Ao explorar essa relação sob uma perspectiva estatística, buscamos contribuir com evidências que podem reforçar a importância de ações mais justas e proporcionais em negociações internacionais sobre clima e desenvolvimento sustentável.

## 📊 Conjunto de Dados Selecionado  
- **Nome do conjunto de dados:**  
CO2 Emissions Country Wise Visualizations

- **Fonte:**
  - Classificação dos paises por continente: [Kaggle - country to continent]
    - https://www.kaggle.com/datasets/statchaitya/country-to-continent/data?select=countryContinent.csv
  - População Mundial [World Population Dataset]
    - https://www.kaggle.com/code/samuelrodriguesagra/estat-stica-atividade
  - Emissões de CO₂ Per Capita: [Kaggle - CO2 Emissions Country Wise] 
    - https://www.kaggle.com/code/odins0n/co2-emissions-country-wise-visualizations/
  - Emissões de CO₂ Total: [Kaggle - CO2 Emissions] 
    - https://www.kaggle.com/datasets/ulrikthygepedersen/co2-emissions-by-country
  - PIB dos países: [World Bank - GDP (current US$)] 
    - https://data.worldbank.org/indicator/NY.GDP.MKTP.CD


- **Descrição breve:**  
O conjunto de dados "CO2 Emissions Country Wise Visualizations" reúne informações sobre as emissões de dióxido de carbono (CO₂) por país ao longo do tempo, com foco no período de 1960 a 2018. O escopo     geográfico é global, cobrindo dezenas de países com dados padronizados. As principais variáveis incluem: emissões anuais de CO₂ por país (em toneladas), emissões per capita, PIB per capita, população e outros indicadores econômicos e ambientais. Este conjunto de dados permite explorar como as emissões evoluíram ao longo das décadas e como elas se comparam entre diferentes países e regiões.

- **Justificativa para a escolha:**  
Este conjunto de dados é ideal para análises estatísticas que relacionem crescimento econômico e impacto ambiental. Ele fornece uma base robusta para investigar a correlação entre PIB per capita e emissões acumuladas de CO₂, o que é essencial para discutir responsabilidade histórica nas mudanças climáticas. Além disso, os dados estão organizados de forma acessível para visualizações e testes estatísticos, o que facilita a construção de evidências sobre desigualdades na contribuição para a crise climática. Essa abordagem é particularmente útil em debates sobre justiça climática e políticas públicas globais.

---

## ❓ Perguntas ou Hipóteses  
Quais países mais emitiram CO₂ ao longo do século XX?

Quais países apresentam os maiores PIBs per capita atualmente?

Existe correlação entre as emissões acumuladas de CO₂ e o PIB per capita atual dos países?

Países que mais poluíram no século XX têm, em média, maior riqueza hoje?

Grupos de países com maior e menor emissão apresentam diferenças estatisticamente significativas no nível de riqueza atual?


## 🔍 Metodologia  

Para responder às perguntas propostas, a análise será conduzida em etapas, combinando técnicas de **estatística descritiva**, **exploratória** e **inferencial**. O processo será estruturado da seguinte forma:  

1. **Tratamento e integração dos dados**  
   - Unificação dos diferentes conjuntos de dados (emissões totais, emissões per capita, PIB, população e classificação por continente e renda) utilizando o **nome do país** como chave de junção.  
   - Padronização de formatos e nomes de variáveis.  
   - Exclusão ou imputação de valores ausentes conforme o caso.  

2. **Análise Exploratória dos Dados (AED)**  
   - Cálculo de **estatísticas descritivas** (média, mediana, desvio padrão, mínimo e máximo) para emissões totais e per capita.  
   - Visualizações gráficas: histogramas, boxplots, gráficos de linhas e barras para observar tendências e comparações entre países e regiões.  

3. **Análises específicas**  
   - **Top emissores globais**: Identificação dos 10 países com maior emissão total no último ano disponível, apresentando valores absolutos.  
   - **Distribuição per capita**: Cálculo e visualização da distribuição das emissões per capita no último ano, destacando dispersão e outliers.  
   - **Variação por continente**: Agrupamento por continente e década para medir variação média e desvio padrão das emissões totais por país, identificando o continente com maior instabilidade ao longo do tempo.  
   - **Tendência global**: Cálculo da média e do desvio padrão das emissões globais por década para observar tendências históricas.  
   - **Discrepância entre total e per capita**: Análise dos 5 países com maior e menor diferença proporcional entre emissões totais e per capita no último ano.  
   - **Distribuição por renda**: Agrupamento por faixas de renda (alta, média, baixa) conforme classificação do Banco Mundial, calculando médias e desvios padrão das emissões per capita.  

4. **Correlação entre emissões e riqueza**  
   - Cálculo do **coeficiente de correlação de Pearson** entre emissões acumuladas de CO₂ e PIB per capita atual.  
   - Interpretação da força e direção da correlação.  
   - Análise de possíveis outliers e padrões regionais.  

5. **Testes de hipótese**  
   - Aplicação de **testes t de Student** ou **ANOVA** (dependendo do número de grupos) para verificar se países com maiores emissões apresentam PIB per capita significativamente diferente dos demais.  
   - Nível de significância adotado: 5% (α = 0,05).  

6. **Ferramentas utilizadas**  
   - **Python** (pandas, numpy, matplotlib, seaborn, scipy) para processamento e visualização.  
   - **Planilhas eletrônicas** para verificações manuais pontuais.  

7. **Interpretação e conclusões**  
   - Discussão dos resultados à luz do conceito de justiça climática.  
   - Comparação dos achados com tendências já conhecidas em relatórios do IPCC e estudos sobre emissões históricas.  

## 🛠️ Ferramentas Utilizadas  

Para a execução do projeto, foram utilizadas as seguintes ferramentas:  

- **Kaggle** – Plataforma para acesso, exploração e download dos conjuntos de dados utilizados.  
- **Jupyter Notebook** – Ambiente interativo para desenvolvimento, execução e documentação do código.  
- **Linguagem Python** – Linguagem principal para tratamento, análise e visualização dos dados.  
- **Biblioteca Pandas** – Utilizada para manipulação e análise de dados tabulares de forma eficiente.  

## 📈 Resultados  

A análise estatística e visual dos dados sobre emissões de CO₂ revelou os seguintes pontos-chave:

1. **Distribuição Global das Emissões per capita (2018)**  
   - Média: **4,06 t/hab**  
   - Mediana: **2,60 t/hab**  
   - Desvio padrão: **4,58 t/hab**  
   - Mínimo: **0,026 t/hab**  
   - Máximo: **32,42 t/hab**  
   O histograma evidenciou forte assimetria à direita, com a maioria dos países emitindo pouco e alguns poucos com emissões extremamente altas. O boxplot confirmou a presença de **outliers** significativos.

2. **Variação das Emissões por Continente e Década**  
   - Nas décadas de **1960 a 1980**, a Europa apresentou a maior variabilidade.  
   - A partir de **1990**, a Ásia assumiu o posto, com aumento expressivo no desvio padrão, atingindo **15,9 milhões kt** em 2010.  
   - Esse crescimento acompanha a industrialização acelerada e expansão econômica asiática.

3. **Tendência da Emissão Média Global (por década)**  
   - Pico observado na década de **1970** (~1241 kt).  
   - Redução até os anos 1990, seguida de leve recuperação nos anos 2000.  
   - O desvio padrão das médias globais caiu ao longo do tempo, indicando menor desigualdade entre países no volume total emitido.

4. **Emissões por Grupo de Renda (2010–2018)**  
   - Alta renda: **8,98 t/hab** (maior média e grande dispersão).  
   - Baixa renda: **0,29 t/hab**.  
   - Renda média baixa: **1,03 t/hab**.  
   - Renda média alta: **3,82 t/hab**.  
   Observa-se relação positiva entre renda e emissões per capita.

5. **Maiores Emissores em 2018 (em valores absolutos)**  
   - **China**: 10,50 Gt  
   - **EUA**: 4,98 Gt  
   - **Índia**: 2,45 Gt  
   - Os 10 maiores emissores somaram **23,84 Gt**, representando parcela significativa do total global.

6. **Discrepância entre Emissões per capita Declaradas e Calculadas**  
   - Maiores discrepâncias: Palau, EAU, Nauru, Islândia, Omã.  
   - Menores discrepâncias: Sri Lanka, Burkina Faso, Antígua e Barbuda, Israel, Etiópia.


## 📌 Conclusões  
Os resultados indicam que há uma correlação positiva significativa entre as emissões acumuladas de CO₂ e o PIB per capita atual, sugerindo que os países que mais cresceram economicamente no século XX também foram os maiores emissores. No entanto, essa relação não é uniforme, pois existem outliers que destacam particularidades regionais e econômicas.

A análise por grupos de renda reforça a disparidade entre países ricos e pobres no que diz respeito às emissões per capita, apontando para um desequilíbrio na responsabilidade histórica sobre as mudanças climáticas. Esses achados fortalecem a argumentação em prol da justiça climática, onde países que mais contribuíram para o aquecimento global deveriam assumir maior responsabilidade em políticas e investimentos ambientais.

## ⚠️ Limitações e Trabalhos Futuros  
Este estudo tem algumas limitações importantes:  
- A qualidade e a abrangência dos dados históricos podem variar entre países, o que pode afetar a precisão das análises.  
- Não foram consideradas variáveis intermediárias, como políticas ambientais, intensidade tecnológica, e mudanças na estrutura econômica dos países.  
- O período analisado vai até 2018, não contemplando eventos recentes que possam alterar tendências.  

Trabalhos futuros podem incluir:  
- Análise mais detalhada de causalidade entre crescimento econômico e emissões, utilizando modelos econométricos avançados.  
- Inclusão de outras variáveis ambientais e sociais para uma análise multidimensional da justiça climática.  
- Estudos regionais mais profundos para entender dinâmicas específicas de continentes e grupos de países.  
- Atualização dos dados com informações mais recentes e projeções para as próximas décadas.

---
