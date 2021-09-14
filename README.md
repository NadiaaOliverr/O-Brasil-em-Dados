# O cenário da Tuberculose no Brasil

![Imagem de uma vacina que não está com a ponta encaixada e logo abaixo, está escrito na cor preta o título do projeto e os integrantes](https://i.imgur.com/XYMsiNj.jpg)

<a name="inicio"></a>
## Sumário

1. [Motivação](#motivacao)
2. [Introdução](#intro)
3. [Perguntas a serem respondidas: Parte 1](#perguntas)
4. [Tratamento de Dados: Parte 2(#parte2)
5. [Referências de Dataset](#refsdata)
6. [Referências Bibliográficas](#refs)
7. [Contribuidores](#colaboradores)

<a name="motivacao"></a>
### Motivação

A tuberculose ainda é a doença infecciosa que mais mata no mundo todo <a href="https://jornal.usp.br/atualidades/tuberculose-e-a-doenca-infecciosa-que-mais-mata-no-mundo/">[1]</a>. Com o avanço da pandemia, os compromissos que foram assumidos para eliminar a tuberculose como problema de saúde estão sendo ameaçados. Segundo alguns <a href="https://portal.fiocruz.br/noticia/pandemia-limita-acoes-para-erradicacao-da-tuberculose">especialistas</a>, a pandemia eliminou doze anos de progressos na luta global contra a tuberculose. 

Em relação ao Brasil, o país continua entre os 30 países de alta carga para tuberculose e para coinfecção TB-HIV, sendo, portanto, considerado prioritário para o controle da doença no mundo pela <a href="https://www.gov.br/saude/pt-br/media/pdf/2021/marco/24/boletim-tuberculose-2021_24.03">Organização Mundial de Saúde (OMS).</a> 

Apesar da Covid-19 estar sendo a principal preocupação, outras doenças transmissíveis como a tuberculose, não devem ser negligenciadas. O intuito do estudo é analisar a doença no Brasil, quais fatores podem aumentar os casos e como a vacinação contra essa doença na infância é necessária. 

<a href="#inicio">Voltar ao Sumário</a>
<a name="intro"></a>
### Introdução

A tuberculose (TB) é uma doença infecciosa potencialmente grave que afeta principalmente os pulmões. A bactéria que causa a tuberculose é transmitida de pessoa para pessoa por meio de pequenas gotículas liberadas no ar por meio de tosses e espirros. A TB se torna ainda mais grave devido a possibilidade de acometer outros órgãos e sistemas.

A forma extrapulmonar - que atinge outras áreas - porém, é mais comum em pacientes com sistema imunológico comprometido, como no caso de pessoas que vivem com HIV, já que enfraquece o sistema imunológico de uma pessoa, esta não pode combater os germes da tuberculose. 
 
Embora seu corpo possa abrigar a bactéria que causa a tuberculose, seu sistema imunológico geralmente pode evitar que você adoeça. Por esse motivo, os médicos fazem uma distinção entre: TB latente no qual existe uma infecção de TB, mas as bactérias no corpo são inativas e não causam sintomas, não é contagiosa porém pode virar TB ativa; TB ativa deixa a pessoa doente e é contagiosa.


<a href="#inicio">Voltar ao Sumário</a>

<a name="perguntas"></a>
# Perguntas a serem respondidas: Parte 1

| Número |                                                 Pergunta                                                 |
|:------:|--------------------------------------------------------------------------------------------------------|
| 1      | Qual período teve a maior taxa de doses aplicadas de Tuberculose?                                        |
| 2      | Quais os estados que mais vacinaram durante os últimos anos?                                             |
| 3      | Qual período teve a menor taxa de doses aplicadas de TB?                                                 |
| 4      | Quais os estados que menos vacinaram durante os últimos anos?                                            |
| 5      | Qual a taxa de incidência de TB por ano?                                                                 |
| 6      | Qual estado teve o maior percentual de vacinação per capta? (Vacina BCG)                                 |
| 7      | Com base nas analises anterioes, o coeficiente de incidência de TB no país aumentou ou diminiu?          |
| 8      | Durante o começo da pandemia em 2020, o número de casos diminiu significamente?                          |
| 9      | Qual a letalidade média por ano da doença?                                                               |
| 10     | Qual estado brasileiro que mais apresenta casos e óbitos da doença durante os últimos anos?              |
| 11     | Existe uma relação entre as doses aplicadas das vacinas e as taxas de incidência e óbito?                |
| 12     | Existe uma relação entre a taxa de pobreza e a incidência de TB?                                         |
| 13     | Há alguma ligação entre o número de população privada de liberdade e o número de casos novos de TB?      |
| 14     | Existe uma relação entre a taxa de incidência de HIV e a de incidência de TB?                            |
| 15     | Qual a porcentagem de casos novos são por conta da infesção por HIV?                                     |
| 16     | Qual a relação entre incidência e cobertura vacinal da TB?                                               |
| 17     | Existe uma relação entre os estados que menos vacinaram e escolaridade?                                  |
| 18     | Existe uma relação entre saneamento básico e incidência de TB?                                           |
| 19     | Em geral como é a situação de tratamento (cura, abandono) da doença nos ultimos anos?                    |
| 20     | O que se pode concluir com as análises feitas?                                                           |

<a href="#inicio">Voltar ao Sumário</a>


<a name="parte2"></a>
# Tratamento de Dados: Parte 2
- Tratar manualmente: o DATASUS dá um texto e depois os dados, e como estamos trabalhando com poucos dados a melhor opção foi fazer isso manualmente do que demorar a fazer uma função para isso. 
- Separar o código de UF da coluna Estado
- Excluir a coluna 2021 de alguns datasets pois a maioria só vão até 2020.
- Passar para int a coluna dos anos.

<a name="refdata"></a>
### Referências de Dataset
Os dados utilizados neste projeto foram obtidos do <a href="http://www2.datasus.gov.br/DATASUS/index.php?area=0202">Tabnet - DATASUS</a>, um banco de dados disponibilizado pelo departamento de informática do Sistema Único de Saúde do Brasil. Entre os dados disponibilizados, encontramos informações de saúde (indicadores de saúde, assistência à saúde, informações epidemiológicas e de morbidade, informações sobre a rede de assistência à saúde, estatísticas vitais, informações demográficas e socioeconômicas) e informações financeiras (referentes aos recursos do Fundo Nacional de Saúde transferidos aos municípios, aos créditos aos prestadores de serviços de saúde, aos orçamentos públicos de saúde declarados pelos Estados, pelo Distrito Federal e pelos Municípios).

Neste projeto os seguintes datasets foram obtidos:

<h4>Imunizações de Tuberculose - desde 2001</h4>
<p>Aplicando os seguintes filtros:</p>
<ul>
  <li>Opção: Doses aplicadas</li>
  <li>Linha: Unidade da Federação</li>
  <li>Coluna: Ano</li>
  <li>Imunobiológicos: Tuberculose</li>
  <li>Período disponível: 2001 - 2021</li>
</ul>

### Dicionário
- Cobertura Vacinal: Esse termo refere-se ao percentual da população que está vacinada. Quanto mais pessoas receberem determinada vacina, maior será a cobertura vacinal. A eliminação ou controle de qualquer doença imunoprevenível depende da obtenção desse índice de sucesso. Um exemplo clássico do resultado de alta cobertura vacinal é o da varíola, doença que assolava o mundo matando aos milhares. Depois do esforço mundial para vacinar praticamente todas as pessoas, o vírus por fim desapareceu e agora a varíola é apenas parte da história. Para acabar com doenças graves, é necessário que a maior parte da população esteja vacinada. Mas para a erradicação ou controle não basta apenas atingir altas coberturas vacinais, é preciso mantê-las até que o agente causador da doença esteja eliminado. Mesmo que em determinado momento ocorram apenas poucos casos de alguma doença graças à vacinação, se a população parar de se vacinar, cada vez mais pessoas ficarão desprotegidas e outras tantas serão infectadas, voltando a espalhar a doença, e assim, em pouco tempo, todo o progresso obtido ao longo dos anos estará perdido.

- Coeficiente/ taxa: Relação entre o número de casos de certa doença ocorridos em uma população ou grupo populacional. O denominador (população) é sempre referenciado como potência de 10 (mil, 100 mil, um milhão). Esta relação é utilizada em Saúde Pública para estimar a probabilidade da ocorrência ou não da doença estudada.

<a href="#inicio">Voltar ao Sumário</a>
<a name="refs"></a>
### Referências Bibliográficas
- <a href="https://www.mayoclinic.org/diseases-conditions/tuberculosis/symptoms-causes/syc-20351250">Tuberculosis</a>
- <a href="https://www.gov.br/saude/pt-br/media/pdf/2021/marco/24/boletim-tuberculose-2021_24.03">Boletim Tuberculose 2021</a>
- <a href="https://www.unicef.org/brazil/comunicados-de-imprensa/pandemia-de-covid-19-leva-a-um-grande-retrocesso-na-vacinacao-infantil">A pandemia de Covid-19 leva a um grande retrocesso na vacinação infantil, mostram novos dados da OMS e do UNICEF </a>
- <a href="https://familia.sbim.org.br/vacinas/conceitos-importantes">Conceitos importantes</a>

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
