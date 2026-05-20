# SINAN_DATASUS
# 📊 Dataset SINAN/DATASUS — Violência Doméstica contra Mulheres em Mato Grosso do Sul

## 📝 Descrição

Este repositório reúne arquivos em formato **CSV** extraídos do **Portal SINAN/DATASUS**, referentes às notificações de violência envolvendo pessoas do sexo feminino no estado de **Mato Grosso do Sul (MS)**.

Os dados abrangem o período de **2015 a 2025** e possuem a mesma estrutura de colunas, permitindo análises temporais, territoriais e epidemiológicas sobre diferentes formas de violência notificadas no sistema de saúde.

O conjunto de dados pode ser utilizado para estudos sobre:

- 🚺 Violência contra a mulher;
- 🏠 Violência doméstica e familiar;
- ⚠️ Violência sexual;
- 📍 Distribuição municipal das notificações;
- 🧬 Perfil sociodemográfico das vítimas;
- 🧑‍⚖️ Relação provável entre vítima e autor da violência;
- 🏥 Encaminhamentos para saúde, assistência social e rede de proteção;
- 📈 Análises exploratórias, estatísticas e preditivas em Ciência de Dados.

> ⚠️ Observação: os dados representam **notificações registradas no sistema de saúde**, não necessariamente a totalidade dos casos ocorridos. Deve-se considerar a possibilidade de subnotificação, inconsistências de preenchimento e variações na qualidade dos registros ao longo dos anos.

---

## 📁 Estrutura dos arquivos

O repositório está organizado com arquivos anuais do SINAN/DATASUS referentes ao estado de Mato Grosso do Sul, no período de **2015 a 2025**.

A estrutura contém dois grupos principais de arquivos:

1. **Base geral feminina**: arquivos com notificações envolvendo pessoas do sexo feminino.
2. **Recorte temático Sexual/Feminicídio**: arquivos filtrados para análise específica de violência sexual e possíveis registros relacionados ao feminicídio.
   
Os arquivos seguem uma estrutura anual, com registros de Mato Grosso do Sul:

```text
Dataset/
├── VIOLBR15_MS_feminino_SEXUAL_FEMINICIDIO.csv
├── VIOLBR16_MS_feminino.csv
├── VIOLBR16_MS_feminino_SEXUAL_FEMINICIDIO.csv
├── VIOLBR17_MS_feminino.csv
├── VIOLBR17_MS_feminino_SEXUAL_FEMINICIDIO.csv
├── VIOLBR18_MS_feminino.csv
├── VIOLBR18_MS_feminino_SEXUAL_FEMINICIDIO.csv
├── VIOLBR19_MS_feminino.csv
├── VIOLBR19_MS_feminino_SEXUAL_FEMINICIDIO.csv
├── VIOLBR20_MS_feminino.csv
├── VIOLBR20_MS_feminino_SEXUAL_FEMINICIDIO.csv
├── VIOLBR21_MS_feminino.csv
├── VIOLBR21_MS_feminino_SEXUAL_FEMINICIDIO.csv
├── VIOLBR22_MS_feminino.csv
├── VIOLBR22_MS_feminino_SEXUAL_FEMINICIDIO.csv
├── VIOLBR23_MS_feminino.csv
├── VIOLBR23_MS_feminino_SEXUAL_FEMINICIDIO.csv
├── VIOLBR24_MS_feminino.csv
├── VIOLBR24_MS_feminino_SEXUAL_FEMINICIDIO.csv
├── VIOLBR25_MS_feminino.csv
└── VIOLBR25_MS_feminino_SEXUAL_FEMINICIDIO.csv

🗂️ Formato dos dados

Os arquivos estão no formato CSV com as seguintes características:

Item	Descrição
📄 Formato	.csv
🔣 Separador	; ponto e vírgula
🔤 Codificação	UTF-8-SIG
📌 Unidade federativa	Mato Grosso do Sul
🧾 Código da UF	50
🚺 Sexo filtrado	Feminino
📆 Período	2015 a 2025
🧱 Estrutura	162 colunas
🧾 Principais grupos de variáveis

A base possui colunas organizadas em blocos temáticos, conforme a estrutura da ficha de notificação do SINAN.

🏥 Identificação da notificação
Campo	Descrição geral
TP_NOT	Tipo de notificação
ID_AGRAVO	Código do agravo notificado
DT_NOTIFIC	Data da notificação
SEM_NOT	Semana epidemiológica da notificação
NU_ANO	Ano da notificação
SG_UF_NOT	UF de notificação
ID_MUNICIP	Código do município de notificação
NOME_MUNICIPIO	Nome do município de notificação
ID_UNIDADE	Unidade notificadora
👩 Perfil da vítima
Campo	Descrição geral
ANO_NASC	Ano de nascimento
NU_IDADE_N	Idade registrada no SINAN
CS_SEXO	Sexo
CS_GESTANT	Situação gestacional
CS_RACA	Raça/cor
CS_ESCOL_N	Escolaridade
SIT_CONJUG	Situação conjugal
ID_OCUPA_N	Ocupação
ORIENT_SEX	Orientação sexual
IDENT_GEN	Identidade de gênero
CICL_VID	Ciclo de vida
📍 Local da ocorrência
Campo	Descrição geral
SG_UF_OCOR	UF de ocorrência
ID_MN_OCOR	Município de ocorrência
DT_OCOR	Data da ocorrência
HORA_OCOR	Hora da ocorrência
LOCAL_OCOR	Local onde ocorreu a violência
LOCAL_ESPE	Especificação do local
OUT_VEZES	Indica se ocorreu outras vezes
⚠️ Tipos de violência
Campo	Descrição geral
VIOL_FISIC	Violência física
VIOL_PSICO	Violência psicológica/moral
VIOL_TORT	Tortura
VIOL_SEXU	Violência sexual
VIOL_TRAF	Tráfico de pessoas
VIOL_FINAN	Violência financeira/econômica
VIOL_NEGLI	Negligência/abandono
VIOL_INFAN	Trabalho infantil
VIOL_LEGAL	Intervenção legal
VIOL_OUTR	Outros tipos de violência
VIOL_ESPEC	Especificação de outra violência
🚨 Violência sexual
Campo	Descrição geral
SEX_ASSEDI	Assédio sexual
SEX_ESTUPR	Estupro
SEX_PUDOR	Atentado violento ao pudor
SEX_PORNO	Pornografia infantil
SEX_EXPLO	Exploração sexual
SEX_OUTRO	Outro tipo de violência sexual
SEX_ESPEC	Especificação da violência sexual
🧍 Relação provável com o autor da violência
Campo	Descrição geral
REL_PAI	Pai
REL_MAE	Mãe
REL_PAD	Padrasto
REL_CONJ	Cônjuge
REL_EXCON	Ex-cônjuge
REL_NAMO	Namorado(a)
REL_EXNAM	Ex-namorado(a)
REL_FILHO	Filho(a)
REL_IRMAO	Irmão(ã)
REL_CONHEC	Conhecido(a)
REL_DESCO	Desconhecido(a)
REL_CUIDA	Cuidador(a)
REL_PATRAO	Patrão/chefe
REL_INST	Pessoa com relação institucional
REL_POL	Policial/agente da lei
REL_OUTROS	Outros vínculos
REL_ESPEC	Especificação do vínculo
👤 Dados sobre o provável autor
Campo	Descrição geral
NUM_ENVOLV	Número de envolvidos
AUTOR_SEXO	Sexo do provável autor
AUTOR_ALCO	Suspeita de uso de álcool pelo autor
🏥 Encaminhamentos e rede de proteção
Campo	Descrição geral
ENC_SAUDE	Encaminhamento à rede de saúde
ENC_TUTELA	Conselho Tutelar
ENC_VARA	Vara da Infância/Juventude
ENC_ABRIGO	Abrigo
ENC_DEAM	Delegacia Especializada de Atendimento à Mulher
ENC_DELEG	Delegacia
ENC_MPU	Ministério Público
ENC_CREAS	CREAS
ENC_IML	Instituto Médico Legal
REDE_SAU	Rede de saúde
ASSIST_SOC	Assistência social
REDE_EDUCA	Rede de educação
ATEND_MULH	Atendimento à mulher
DELEG_MULH	Delegacia da mulher
DEFEN_PUBL	Defensoria Pública
🔢 Códigos frequentes

Muitas variáveis do SINAN utilizam codificação numérica. Em vários campos dicotômicos, a leitura costuma seguir o padrão:

Código	Significado
1	Sim
2	Não
9	Ignorado
vazio / NaN	Não informado ou não preenchido

⚠️ Recomenda-se consultar o dicionário oficial do SINAN para interpretação completa de cada variável.
📌 Observações metodológicas

Este dataset deve ser interpretado com cautela, pois os registros do SINAN correspondem a notificações realizadas pelos serviços de saúde.

Assim, os dados não devem ser entendidos como o número real absoluto de casos de violência contra mulheres no estado, pois podem existir:

subnotificação;
atraso no registro;
campos não preenchidos;
preenchimento como “ignorado”;
divergência entre data da ocorrência e data da notificação;
mudanças nos fluxos de notificação ao longo do tempo;
diferenças municipais na capacidade de registro e vigilância.
🔐 Ética e uso responsável

Embora os arquivos analisados não contenham nome da vítima, o tema envolve dados sensíveis sobre violência. Por isso, recomenda-se:

não tentar reidentificar pessoas;
não cruzar os dados com bases que possam expor vítimas;
evitar divulgação de microdados em recortes muito pequenos;
utilizar os dados apenas para fins científicos, educacionais, jornalísticos, institucionais ou de políticas públicas;
respeitar princípios de privacidade, segurança da informação e proteção de dados.
🎯 Finalidade do repositório

Este repositório tem como objetivo apoiar análises de dados sobre violência contra mulheres em Mato Grosso do Sul, contribuindo para:

📚 pesquisas acadêmicas;
🧠 projetos de Ciência de Dados;
📊 painéis de visualização;
🏛️ estudos sobre políticas públicas;
🚨 monitoramento territorial da violência;
🤖 aplicações de mineração de dados e aprendizado de máquina;
🧩 compreensão dos padrões de notificação no sistema de saúde.
🛠️ Tecnologias recomendadas

Para análise dos dados, recomenda-se o uso de:

Python;
Pandas;
NumPy;
Matplotlib;
Seaborn;
Plotly;
Jupyter Notebook;
Power BI;
Excel;
QGIS ou GeoPandas para análises espaciais.
📚 Fonte dos dados

Os dados são provenientes do Sistema de Informação de Agravos de Notificação — SINAN, disponibilizado pelo DATASUS/Ministério da Saúde, referentes ao agravo de Violência Interpessoal/Autoprovocada.

⚖️ Licença e responsabilidade

Este repositório utiliza dados públicos para fins de estudo, pesquisa e análise. O uso das informações é de responsabilidade de quem realiza a análise.

Recomenda-se citar a fonte original dos dados em trabalhos acadêmicos, relatórios técnicos, painéis públicos ou publicações derivadas.

👨‍💻 Autor

Projeto organizado para fins de estudo em Ciência de Dados, com foco na análise da violência contra mulheres no estado de Mato Grosso do Sul.

💡 Possíveis próximos passos
 Criar notebook de análise exploratória;
 Gerar painel anual de notificações;
 Mapear municípios com maior número de registros;
 Criar indicadores por tipo de violência;
 Analisar vínculo entre vítima e provável autor;
 Estudar padrões de violência sexual;
 Integrar dados populacionais do IBGE;
 Calcular taxas por 100 mil mulheres;
 Criar visualizações geográficas;
 Desenvolver modelos preditivos para identificação de padrões de risco.
🧭 Aviso importante

Este dataset não deve ser usado para julgamento individual, exposição de vítimas ou conclusões simplistas. A violência contra mulheres é um fenômeno social complexo, atravessado por fatores culturais, econômicos, territoriais, institucionais e históricos.

A análise dos dados deve ser feita com responsabilidade técnica, sensibilidade social e compromisso com a proteção das vítimas.

## 📚 Fonte dos dados

Os dados utilizados neste repositório foram obtidos a partir dos microdados públicos do **SINAN/DATASUS**, referentes ao agravo **Violência doméstica, sexual e/ou outras violências**.

A consulta dos arquivos foi realizada por meio do catálogo:

🔗 **Alpaca / Quantilica — Dados Públicos**  
https://alpaca.quantilica.com/dados

🔗 **SINAN-VIOL — Violência doméstica, sexual e/ou outras violências**  
https://alpaca.quantilica.com/dados/sinan-viol

Os arquivos originais estão disponíveis no FTP público do DATASUS, em formato `.dbc`, na base nacional `VIOLBR`, correspondente aos microdados do SINAN sobre violência interpessoal/autoprovocada.

---

## 🏛️ Origem institucional

| Item | Descrição |
|---|---|
| 🏛️ Sistema | SINAN — Sistema de Informação de Agravos de Notificação |
| 🏥 Órgão responsável | Ministério da Saúde / DATASUS |
| 📂 Base | SINAN-VIOL |
| 📌 Agravo | Violência doméstica, sexual e/ou outras violências |
| 🌎 Abrangência original | Brasil |
| 📍 Recorte deste repositório | Mato Grosso do Sul |
| 🚺 Filtro aplicado | Sexo feminino |
| 📆 Período analisado | 2015 a 2025 |
| 📄 Formato original | `.dbc` |
| 📄 Formato disponibilizado neste repositório | `.csv` |

---

## 🗃️ Arquivos originais consultados SINAN DATASUS

Os arquivos originais do DATASUS estão organizados por ano. Neste repositório, foram utilizados os arquivos referentes ao período de **2015 a 2025**, com posterior conversão, filtragem e organização em arquivos CSV.

| Ano | Arquivo original DATASUS | Tipo da base | Situação |
|---|---|---|---|
| 2015 | `VIOLBR15.dbc` | Final | Não preliminar |
| 2016 | `VIOLBR16.dbc` | Final | Não preliminar |
| 2017 | `VIOLBR17.dbc` | Final | Não preliminar |
| 2018 | `VIOLBR18.dbc` | Final | Não preliminar |
| 2019 | `VIOLBR19.dbc` | Final | Não preliminar |
| 2020 | `VIOLBR20.dbc` | Final | Não preliminar |
| 2021 | `VIOLBR21.dbc` | Final | Não preliminar |
| 2022 | `VIOLBR22.dbc` | Final | Não preliminar |
| 2023 | `VIOLBR23.dbc` | Final | Não preliminar |
| 2024 | `VIOLBR24.dbc` | Final | Não preliminar |
| 2025 | `VIOLBR25.dbc` | Preliminar | Sim |

---

## 🔗 Endereços FTP dos arquivos originais

```text
ftp://ftp.datasus.gov.br/dissemin/publicos/SINAN/DADOS/FINAIS/VIOLBR15.dbc
ftp://ftp.datasus.gov.br/dissemin/publicos/SINAN/DADOS/FINAIS/VIOLBR16.dbc
ftp://ftp.datasus.gov.br/dissemin/publicos/SINAN/DADOS/FINAIS/VIOLBR17.dbc
ftp://ftp.datasus.gov.br/dissemin/publicos/SINAN/DADOS/FINAIS/VIOLBR18.dbc
ftp://ftp.datasus.gov.br/dissemin/publicos/SINAN/DADOS/FINAIS/VIOLBR19.dbc
ftp://ftp.datasus.gov.br/dissemin/publicos/SINAN/DADOS/FINAIS/VIOLBR20.dbc
ftp://ftp.datasus.gov.br/dissemin/publicos/SINAN/DADOS/FINAIS/VIOLBR21.dbc
ftp://ftp.datasus.gov.br/dissemin/publicos/SINAN/DADOS/FINAIS/VIOLBR22.dbc
ftp://ftp.datasus.gov.br/dissemin/publicos/SINAN/DADOS/FINAIS/VIOLBR23.dbc
ftp://ftp.datasus.gov.br/dissemin/publicos/SINAN/DADOS/FINAIS/VIOLBR24.dbc
ftp://ftp.datasus.gov.br/dissemin/publicos/SINAN/DADOS/PRELIM/VIOLBR25.dbc

⚠️ Observação sobre a base de 2025

O arquivo de 2025 é identificado como preliminar no catálogo de origem. Portanto, os registros desse ano podem sofrer alterações, revisões ou atualizações posteriores pelo DATASUS.

Por esse motivo, análises envolvendo o ano de 2025 devem ser interpretadas com cautela, especialmente em comparações históricas, séries temporais e construção de indicadores epidemiológicos.

🔄 Processamento realizado

A base original do DATASUS foi disponibilizada em formato .dbc. Para este repositório, os dados foram processados e organizados em formato .csv, com os seguintes recortes:

📍 seleção de registros do estado de Mato Grosso do Sul;
🚺 seleção de registros referentes ao sexo feminino;
📆 separação dos arquivos por ano;
🧩 criação de recortes temáticos sobre violência sexual e feminicídio;
📊 organização dos arquivos para uso em análises com Python, Excel, Power BI e outras ferramentas de Ciência de Dados.
📌 Como citar a fonte dos dados

Sugestão de citação da fonte no próprio projeto:

BRASIL. Ministério da Saúde. DATASUS. Sistema de Informação de Agravos de Notificação — SINAN. Microdados de Violência doméstica, sexual e/ou outras violências. Disponível em: https://alpaca.quantilica.com/dados/sinan-viol. Acesso em: data de consulta.

🧭 Aviso metodológico

Os dados analisados correspondem a notificações registradas no sistema de saúde, e não necessariamente ao número total real de casos de violência contra mulheres. A interpretação dos resultados deve considerar possíveis subnotificações, atrasos de registro, campos ignorados, ausência de preenchimento e diferenças na capacidade de notificação entre municípios e anos.
