# Iniciação Científica - Redes Neurais

## Descrição do Projeto:
<p align = "justify">
    Este projeto de pesquisa tem como objetivo desenvolver um modelo de cálculo estimado do déficit habitacional no município de Jacareí-SP, utilizando técnicas de Redes Neurais Artificiais (RNA) para tratar dados censitários e inferir a distribuição espacial do déficit habitacional em escalas intraurbanas, como setores censitários (que compõem uma Área de Ponderação). O déficit habitacional é analisado a partir de seus quatro componentes principais:
</p> 

- Domicílios precários;
- Adensamento excessivo de moradores em domicílios alugados;
- Ônus excessivo com aluguel;
- Coabitação familiar não desejada.

<p align = "justify">
    A partir da boa predição do défict, com dados não ideais, das Áreas de Ponderação, poderia-se inferir um resultado aproximado para seus respectivos Setores Censitários. Dessa form, a pesquisa visa gerar dados detalhados em nível intraurbano, permitindo análises mais precisas e auxiliando os planejadores urbanos na formulação de políticas públicas habitacionais.
</p> 

## Metodologia:
<p align = "justify">
    O projeto utiliza dados do Censo Demográfico 2010 (e possivelmente do Censo 2022, dependendo da disponibilidade) para calcular o déficit habitacional. A metodologia inclui:  
    <ol>
        <li>Cálculo do déficit habitacional por método direto, utilizando microdados do Censo Demográfico para todas as Áreas de Ponderação do estado de São Paulo.</li>
        <li>Aplicação do Principal Components Analisys (PCA) nos atributos comuns a Áreas de Ponderação e Setores Censitários (atributos não ideais e que não fazem parte do cálculo de défict)</li>
        <li>Aplicação de Redes Neurais Artificiais para estimar o déficit habitacional utilizando a redução dimensional anterior.</li>
        <li>Análise espacial do déficit habitacional, permitindo a visualização da distribuição do fenômeno em escalas intraurbanas.</li>
    </ol> 
</p>

## Resultado Esperado:
<p align = "justify">
    Estimativa do déficit habitacional em setores censitários utilizando a mesma Rede Neural treinada para Áreas de Ponderação, permitindo uma análise espacial detalhada.
</p>

## Resultado Obtido:
<p align = "justify">
    A regressão feita pela Rede Neural não foi satisfatória, obtendo uma porcentagem média do erro absoluto em relação à grandeza de 75%, 71%, 34% e 19% para Domicílios Precários, Adensamento Excessivo, Ônus Excessivo e Coabitação Familiar, respectivamente.
</p>

<p align = "justify">
    Ou seja, tomando como exemplo os Domicílios Precários, em média, a diferença entre a predição da Rede Neural e o valor real representava 75% do valor real de défict.
</p>

## Possíveis Estratégias a se Seguir:
- Fazer um filtro com análise qualitativa das variáveis;
- Buscar outras variáveis mais explicativas de outras bases;
- Compor variáveis para obter outras;
- Tratamento das variáveis explicativas (normalização, eliminação de outliers, etc);

## Licença:
[MIT](https://choosealicense.com/licenses/mit/)

Título: O uso de Redes Neurais para estimativa do déficit habitacional intramunicipal: Jacareí como estudo de caso  
Autor: Allan Moreira de Almeida   
Orientador: Elza Luli Miyasaka  
Instituição: Universidade Federal de São Carlos (UFSCar)  
Ano: 2023