
[![Build
Status](https://travis-ci.com/liibre/coronabr.svg?branch=master)](https://travis-ci.com/liibre/coronabr)

# Download de dados de COVID-19 no Brasil

<img src="https://raw.githubusercontent.com/liibre/coronabr/master/vignettes/figs/liibre.png" align="right" alt="" width="120" />

**coronabr** é um pacote de [R](https://www.r-project.org/) para fazer
*download* e visualizar os dados dos casos diários de coronavírus
(COVID-19) disponibilizados por diferentes fontes:

-   [Ministério da
    Saúde](http://plataforma.saude.gov.br/novocoronavirus/#COVID-19-brazil);
-   [Brasil I/O](https://brasil.io/dataset/covid19/caso);
-   [Johns Hopkins
    University](https://github.com/CSSEGISandData/COVID-19)

## Nosso objetivo

O nosso objetivo é facilitar o acesso aos dados de diferentes fontes,
usando ferramentas de acesso aberto e que permitam reprodutibilidade.

O código é aberto. Entre em [como
usar](https://liibre.github.io/coronabr/articles/coronabr.html) para um
exemplo de como utilizar o pacote. Compartilhe.

Fazemos ciência aberta, democrática e reprodutível. Este é um trabalho
em desenvolvimento. Para entender como contribuir, clique
[aqui](https://liibre.github.io/coronabr/CONTRIBUTING.html).

## Aviso!

Disponibilizamos aqui atualizações dos gráficos. Sabemos que deve haver
maneiras responsáveis de apresentar estes dados e que as comparações
entre regiões e países dependem de muitas variáveis.

Os dados são referentes aos casos notificados. É sabido que temos
subnotificação e atraso nas notificações. Assim, mais do que nunca, não
refletem a epidemia em si.

## Sobre os dados

Antes de mais nada, declaramos nossa postura alinhada com as ideias de
uma ciência de dados responsável, compromissada e feminista. Somos
pessoas alinhadas com o [manifest-no](https://www.manifestno.com/),
refutamos regimes de dados prejudiciais e nos comprometemos a novos
futuros de dados.

Apesar de acreditarmos no acesso sem distinção a dados abertos, não
recomendamos que toda análise que possa ser feita o seja. Ao se tratar
de uma situação de saúde pública delicada, visualizações, extrapolações,
e predições devem ser feitas com todo cuidado, lembrando que a qualidade
dos dados é incerta e que todo dado diz respeito a uma pessoa.

No Brasil, a notificação de casos carrega consigo vieses espaciais,
econômicos e de classe que não podem ser ignorados. Para ver modelos
**responsáveis** de previsão do crescimento no número de casos veja o
[Observatório COVID-19 Brasil](https://covid19br.github.io/index.html)
(um grupo colaborativo de pessoas cientistas brasileiras) e o [Mapa de
previsão da propagação da COVID-19 por contágio comunitário no
Brasil](https://covid-19-risk.github.io/map/brazil/pt/).

### Nota sobre os dados disponibilizados pelo Ministério da Saúde

-   A partir de 2020-03-14, a notificação de casos graves de COVID-19
    foca apenas nos casos graves que são atendidos nos hospitais.
-   Até 2020-03-18 o ministério de saúde brasileiro disponibilizou os
    dados de casos de coronavirus COVID-19 discriminados por estado na
    página
    <http://plataforma.saude.gov.br/novocoronavirus/#COVID-19-brazil>
-   Entre 2020-03-18 e 2020-03-25, a página original do Ministério da
    Saúde parou de funcionar e os dados de casos de coronavirus COVID-19
    discriminados por estado foram divulgados em apresentações de
    powerpoint e PDFs no blog do Ministério. [Adriano
    Belisario](https://www.twitter.com/belisards) fez a compilação
    manual destes dados [neste
    repositório](https://github.com/belisards/coronabr)
-   A partir de 2020-03-26 o Ministério de Saúde brasileiro
    disponibilizou os dados de casos de coronavirus COVID-19 na página
    <https://covid.saude.gov.br/>
-   A partir de 2020-03-28 a opção de fazer *download* da série
    histórica por casos voltou a estar disponível. Depois disso, o
    padrão tem mudado frequentemente, inclusive no formato de
    disponibilização dos dados que agora é em .xls e não mais .csv.
    Neste momento, temos uma função estável `get_corona_minsaude()` para
    o *download* desses dados (instruções de como usar
    [aqui](https://liibre.github.io/coronabr/articles/minsaude.html)).

## Visualizando os dados

Importante lembrar que desde 2020-03-27 tem muitos testes sem resultados
e que os dados não refletem a epidemia e sim as notificações - e que
essas estão atrasadas devido ao atraso no resultado dos testes.

Entre [aqui](https://liibre.github.io/coronabr/articles/lac.html) para
acompanhar os casos na América Latina (versão em espanhol
[aqui](https://liibre.github.io/coronabr/articles/lac_es.html))

### Crescimento nacional no número de casos de COVID-19

<img src="https://raw.githubusercontent.com/liibre/coronabr/master/docs/articles/articles/graficos_files/figure-html/fig-casos-1.png" align="center" alt="" width="600" />

### Entendendo o aumento diário de COVID-19

<img src="https://raw.githubusercontent.com/liibre/coronabr/master/docs/articles/articles/graficos_files/figure-html/fig-perc-1.png" align="center" alt="" width="600" />

### Crescimento do número de casos de COVID-19 nos estados mais afetados

<img src="https://raw.githubusercontent.com/liibre/coronabr/master/docs/articles/articles/graficos_files/figure-html/estados-1.png" align="center" alt="" width="600" />

<!---
### Número de casos por estado brasileiro

<img src="https://raw.githubusercontent.com/liibre/coronabr/master/docs/articlfes/graficos_files/figure-html/mapa1-1.png" align="center" alt="" width="600" />

### Evolução do número de casos por estado

<img src="https://raw.githubusercontent.com/liibre/coronabr/master/vignettes/figs/anim.gif" align="center" alt="" width="600" />

-->

## Para saber mais:

-   [Observatório Covid-19 BR](https://covid19br.github.io/)

-   Dados compilados pelo Brasil I/O, [Álvaro
    Justen](https://github.com/turicas/) e colaboradores
    [aqui](https://brasil.io/dataset/covid19/caso)

-   [John Hopkins Coronavirus COVID-19 Global
    Cases](https://coronavirus.jhu.edu/map.html)

-   [Mapa de previsão da propagação da COVID-19 por contágio comunitário
    no Brasil](https://covid-19-risk.github.io/map/brazil/pt/)

-   [covid19br](https://paternogbc.github.io/covid19br/index.html), o
    pacote de R [Gustavo Palermo](https://github.com/paternogbc) para
    acompanhar os dados de novos casos no Brasil

-   [Portal da Fiocruz](https://portal.fiocruz.br/coronavirus)

-   [Site oficial da Organização Mundial da Saúde (em
    inglês)](https://www.who.int/emergencies/diseases/novel-coronavirus-2019)

-   [Tira dúvidas do Instituto
    Butantan](http://coronavirus.butantan.gov.br/)

-   [Banco de dados aberto COVID-19 (em
    inglês)](https://pages.semanticscholar.org/coronavirus-research%5D)

-   [Atualização mundial do número de
    casos](https://www.worldometers.info/coronavirus/)

-   [Dez considerações antes de criar mais um gráfico sobre o COVID-19
    (em
    inglês)](https://medium.com/nightingale/ten-considerations-before-you-create-another-chart-about-covid-19-27d3bd691be8)

-   Siga o **Atila Iamarino** no
    [youtube](https://www.youtube.com/channel/UCSTlOTcyUmzvhQi6F8lFi5w),
    [Instagram](www.instagram.com/oatila),
    [twitter](https://twitter.com/oatila) ou
    [telegram](https://t.me/corona_atila). Tem também um [fórum
    brasileiro de reddit](https://www.reddit.com/r/coronabr/) com muita
    informação.

-   Siga também o canal **Peixe Babel** no
    [GitHub](https://github.com/peixebabel),
    [youtube](https://www.youtube.com/CanalPeixeBabel),
    [twitter](https://twitter.com/canalpeixebabel),
    [Instagram](https://www.instagram.com/canalpeixebabel/).

Dúvidas, contribuições e sugestões, poste um *issue*
[aqui](https://github.com/liibre/coronabr/issues), escreva-nos um
[e-mail](mailto:liibrelab@gmail.com) ou nos encontre no twitter
([Sara](https://twitter.com/mortarasara),
[Andrea](https://twitter.com/SanchezTapiaA) ou
[Karlo](https://twitter.com/kguidonimartins)).
