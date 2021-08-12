# Doenças que voltaram a ameaçar o Brasil: uma análise da Sarampo, Rubéola e Poliomielite :bar_chart:

![Imagem de uma vacina que não está com a ponta encaixada e logo abaixo, está escrito na cor preta o título do projeto e os integrantes](https://i.imgur.com/oUYpOSc.jpg)

<a name="inicio"></a>
## Sumário

1. [Motivação](#motivacao)
2. [Introdução](#intro)
3. [Perguntas a serem respondidas](#perguntas)
4. [Referências de Dataset](#refsdata)
5. [Referências Bibliográficas](#refs)
6. [Contribuidores](#colaboradores)

<a name="motivacao"></a>
### Motivação

Devido ao cenário pandêmico que se instaurou desde 2019 através do vírus da Sars-CoV-2 (Covid 19), doenças que estavam erradicadas começaram a surgir novamente em território nacional, como é o caso do Sarampo, que notificou mais de dez mil casos nos últimos anos. Tendo como base esse cenário, o atual estudo tem como objetivo analisar e entender o comportamento de doenças consideradas erradicadas ao longo dos anos, tendo como foco três principais: Sarampo, Rubéola e Poliomielite.

<a href="#inicio">Voltar ao Sumário</a>
<a name="intro"></a>
### Introdução

A Poliomielite, também chamada de pólio ou paralisia infantil, é uma doença contagiosa aguda causada pelo poliovírus, que pode infectar crianças e adultos por meio do contato direto com fezes ou com secreções eliminadas pela boca das pessoas doentes e provocar ou não paralisia. 

Por outro lado, a Rubéola  é uma doença aguda, de alta contagiosidade, que é transmitida pelo vírus do gênero Rubivirus e  pode se espalhar pelo contato direto com a saliva ou o muco de uma pessoa infectada ou pelo ar, por meio de gotículas respiratórias produzidas ao tossir ou espirrar.

E o Sarampo, que sua transmissão ocorre quando o doente tosse, fala, espirra ou respira próximo de outras pessoas. A única maneira de evitar o sarampo é pela vacina.

<a href="#inicio">Voltar ao Sumário</a>

<a name="perguntas"></a>
### Perguntas a serem respondidas

| Número |                                                 Pergunta                                                 |
|:------:|--------------------------------------------------------------------------------------------------------|
| 1      | Qual ano houve maior taxa de doses aplicadas em Sarampo?                                                 |
| 2      | Qual ano houve maior taxa de doses aplicadas em Rubéola?                                                 |
| 3      | Qual ano houve maior taxa de doses aplicadas em Poliomielite?                                            |
| 4      | Qual a porcentagem da população que foi vacinada em Sarampo?                                             |
| 5      | Qual a porcentagem da população que foi vacinada em Rubéola?                                             |
| 6      | Qual a porcentagem da população que foi vacinada em Poliomielite?                                        |
| 7      | Qual a letalidade média de cada uma das doenças?                                                         |
| 8      | Qual região brasileira mais apresenta casos e óbitos de cada doença?                                     |
| 9      | Quais os estados que menos vacinaram em 2019?                                                            |
| 10     | Qual a taxa de incidência de cada uma das doenças por ano?                                               |
| 11     | Existe uma relação entre as doses aplicadas das vacinas e as taxas de incidência e óbito?                |
| 12     | Existe uma relação entre a taxa de pessoas que possuem saneamento básico e a incidência de Poliomielite? |
| 13     | Qual a taxa de abandono por ano das doenças?                                                             |
| 14     | Qual estado teve menor taxa de abandono?                                                                 |
| 15     | Existe uma relação entre taxa de abandono e escolaridade?                                                |
| 16     | Qual a quantidade de doses aplicadas por região por faixa etária?                                        |
| 17     | Qual a relação entre incidência e cobertura vacinal da Sarampo?                                          |
| 18     | Qual a relação entre incidência e cobertura vacinal da Rubéola?                                          |
| 19     | Qual a relação entre incidência e cobertura vacinal da Poliomielite?                                     |
| 20     | O que se pode concluir com as análises feitas?                                                           |

<a href="#inicio">Voltar ao Sumário</a>


<a name="refdata"></a>
### Referências de Dataset
Os dados utilizados neste projeto foram obtidos do <a href="http://www2.datasus.gov.br/DATASUS/index.php?area=0202">Tabnet - DATASUS</a>, um banco de dados disponibilizado pelo departamento de informática do Sistema Único de Saúde do Brasil. Entre os dados disponibilizados, encontramos informações de saúde (indicadores de saúde, assistência à saúde, informações epidemiológicas e de morbidade, informações sobre a rede de assistência à saúde, estatísticas vitais, informações demográficas e socioeconômicas) e informações financeiras (referentes aos recursos do Fundo Nacional de Saúde transferidos aos municípios, aos créditos aos prestadores de serviços de saúde, aos orçamentos públicos de saúde declarados pelos Estados, pelo Distrito Federal e pelos Municípios).

Neste projeto os seguintes datasets foram obtidos:

<h4>Imunizações de Sarampo - desde 1994</h4>
<p>Aplicando os seguintes filtros:</p>
<ul>
  <li>Opção: Doses aplicadas</li>
  <li>Linha: Unidade da Federação</li>
  <li>Coluna: Ano</li>
  <li>Imunobiológicos: Sarampo</li>
  <li>Período disponível: 1994 - 2019</li>
</ul>

<h4>Imunizações de Rubéola - desde 1994</h4>
<p>Aplicando os seguintes filtros:</p>
<ul>
  <li>Opção: Doses aplicadas</li>
  <li>Linha: Unidade da Federação</li>
  <li>Coluna: Ano</li>
  <li>Imunobiológicos: Rubéola</li>
  <li>Período disponível: 1994 - 2019</li>
</ul>

<h4>Imunizações de Poliomielite - desde 1994</h4>
<p>Aplicando os seguintes filtros:</p>
<ul>
  <li>Opção: Doses aplicadas</li>
  <li>Linha: Unidade da Federação</li>
  <li>Coluna: Ano</li>
  <li>Imunobiológicos: Poliomielite</li>
  <li>Período disponível: 1994 - 2019</li>
</ul>


<a href="#inicio">Voltar ao Sumário</a>
<a name="refs"></a>
### Referências Bibliográficas
- <a href="https://www.unimedfortaleza.com.br/blog/cuidar-de-voce/movimento-antivacina">Movimento antivacina: 4 doenças erradicadas que podem retornar ao Brasil</a>
- <a href="https://www.agenciabrasilia.df.gov.br/2020/11/08/cobertura-vacinal-de-473-contra-poliomielite-ainda-reflete-baixa/">Cobertura vacinal de 47,3% contra poliomielite ainda reflete baixa</a>
- <a href="https://revistacrescer.globo.com/Voce-precisa-saber/noticia/2017/05/grupos-de-pais-contra-vacinas-quais-sao-os-riscos.html">Grupos de pais contra as vacinas: quais são os riscos?</a>
- <a href="http://www.femipa.org.br/noticias/sarampo-polio-difteria-por-que-doencas-erradicadas-estao-voltando/">Sarampo, pólio, difteria… Por que doenças erradicadas estão voltando?</a>

<a name="colaboradores"></a>
### Contribuidores

<table>
  <tr>
    <td align="center"><a href="https://github.com/hpbd152"><img src="https://avatars.githubusercontent.com/u/31517090?v=4" width="100px;" alt=""/><br /><sub><b>Henrique Diniz</b></sub></a><br /><a href="https://github.com/hpbd152" title="Code">💻</a></td>
    <td align="center"><a href="https://github.com/NadiaaOliverr"><img src="https://avatars2.githubusercontent.com/u/41811634?v=4" width="100px;" alt=""/><br /><sub><b>Nádia Oliveira</b></sub></a><br /><a href="https://github.com/NadiaaOliverr" title="Code">💻</a></td>
    <td align="center"><a href="https://github.com/natalicarmo"><img src="https://avatars.githubusercontent.com/u/50000533?v=4" width="100px;" alt=""/><br /><sub><b>Natália Camillo</b></sub></a><br /><a href="https://github.com/natalicarmo" title="Code">💻</a></td>
  </tr>
</table>
<a href="#inicio">Voltar ao Sumário</a>
