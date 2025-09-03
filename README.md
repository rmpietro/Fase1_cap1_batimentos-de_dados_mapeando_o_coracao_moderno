# FIAP - Faculdade de Informática e Administração Paulista

<p align="center">
<a href= "https://www.fiap.com.br/"><img src="assets/logo-fiap.png" alt="FIAP - Faculdade de Informática e Admnistração Paulista" border="0" width=40% height=40%></a>
</p>

<br>

# Cap 1 - Batimentos de Dados – Mapeando o Coração Moderno

## Grupo 50

## 👨‍🎓 Integrantes:

- Gustavo Valtrick - RM559575
- Iago Cotta - RM559655
- Pedro Scofield - RM560589
- Rodrigo Mastropietro - RM560081
- Tiago de Andrade Bastos - RM560467

## 👩‍🏫 Professores:

### Tutor(a)

- <a href="">Leonardo Ruiz Orabona</a>

### Coordenador(a)

- <a href="https://www.linkedin.com/in/profandregodoi/">André Godoi</a>

## 📜 Descrição

Este projeto agrega e define os dados fundamentais a partir de repositórios e bases de dados cardiológicos disponíveis online e se apresenta em três formatos:

- Dados numéricos (simulados ou reais) relacionados a pacientes cardíacos;
- Textos médicos ou literários relacionados à saúde cardiovascular;
- Imagens médicas que representem exames ou sinais visuais do coração.

### 1. Dados numéricos:

Foram adicionados ao repositório dois datasets relacionados e com dados diretamente relacionados porém cujos registros referem-se a pacientes distintos e em momentos diferentes no tempo e espaço:

- [assets/datasets/Cardiovascular_Disease.csv](assets/datasets/Cardiovascular_Disease.csv)
- [assets/datasets/CVD_Risk_Prediction.csv](assets/datasets/CVD_Risk_Prediction.csv)

Esses arquivos estão disponíveis tanto **NESTE REPOSITÓRIO** como no seguinte link para download:

- [Google Drive](https://drive.google.com/drive/folders/1qc77y52Pok4xuj9DwPLPNEdPdkZaHi4F?usp=sharing)

Abaixo, a descrição de ambos os datasets e seus atributos:

1.1. **Cardiovascular_Disease.csv**

Este dataset de doenças cardíacas é proveniente de um dos hospitais multiespecializados na Índia. Contém 14 características (features) comuns. Consiste em 1000 indivíduos analisados e cujos dados são apresentados de forma anonimizada.

**Descrição de atributos (features)**:

| Nº  | Atributo                                       | Código Atribuído  | Unidade                                                                                                                                                                                                                                        | Tipo de Dados |
| --- | ---------------------------------------------- | ----------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------- |
| 1   | Número de Identificação do Paciente            | patientid         | Número                                                                                                                                                                                                                                         | Numérico      |
| 2   | Idade                                          | age               | Em Anos                                                                                                                                                                                                                                        | Numérico      |
| 3   | Gênero                                         | gender            | 1,0 (0= feminino, 1 = masculino)                                                                                                                                                                                                               | Binário       |
| 4   | Tipo de dor no peito                           | chestpain         | 0,1,2,3<br>(Valor 0: angina típica<br>Valor 1: angina atípica<br>Valor 2: dor não anginosa<br>Valor 3: assintomático)                                                                                                                          | Nominal       |
| 5   | Pressão arterial em repouso                    | restingBP         | 94-200 (em mm HG)                                                                                                                                                                                                                              | Numérico      |
| 6   | Colesterol sérico                              | serumcholestrol   | 126-564 (em mg/dl)                                                                                                                                                                                                                             | Numérico      |
| 7   | Açúcar no sangue em jejum                      | fastingbloodsugar | 0,1 > 120 mg/dl<br>(0 = falso, 1 = verdadeiro)                                                                                                                                                                                                 | Binário       |
| 8   | Resultados do eletrocardiograma em repouso     | restingrelectro   | 0,1,2<br>(Valor 0: normal<br>Valor 1: tendo anormalidade da onda ST-T (inversões da onda T e/ou elevação ou depressão ST de > 0,05 mV)<br>Valor 2: mostrando provável ou definitiva hipertrofia ventricular esquerda pelos critérios de Estes) | Nominal       |
| 9   | Frequência cardíaca máxima alcançada           | maxheartrate      | 71-202                                                                                                                                                                                                                                         | Numérico      |
| 10  | Angina induzida por exercício                  | exerciseangia     | 0,1 (0 = não, 1 = sim)                                                                                                                                                                                                                         | Binário       |
| 11  | Oldpeak = ST                                   | oldpeak           | 0-6,2                                                                                                                                                                                                                                          | Numérico      |
| 12  | Inclinação do segmento ST do pico de exercício | slope             | 1,2,3<br>(1-ascendente, 2-plana, 3-descendente)                                                                                                                                                                                                | Nominal       |
| 13  | Número de vasos principais                     | noofmajorvessels  | 0,1,2,3                                                                                                                                                                                                                                        | Numérico      |
| 14  | Classificação                                  | target            | 0,1 (0= Ausência de Doença Cardíaca, 1= Presença de Doença Cardíaca)                                                                                                                                                                           | Binário       |

1.2. **CVD_Risk_Prediction.csv**

Baseado no Sistema de Vigilância de Fatores de Risco Comportamental (BRFSS) do CDC / EUA. Feito por meio de coleta telefônica, seu objetivo é servir à predição de risco de doenças cardíacas com base em fatores demográficos, comportamentais e de saúde. Consta de 308855 registros.

**Descrição de Atributos(features)**:

| Nº  | Variável                         | Tipo       | Valores/Faixa                                                                                                     | Descrição Detalhada                                                                                                                                                                  |
| --- | -------------------------------- | ---------- | ----------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 1   | **General_Health**               | Categórico | "Poor", "Fair", "Good", "Very Good", "Excellent"                                                                  | **Saúde Geral Autorrelatada**<br>Autopercepção do estado geral de saúde do respondente<br>• Excelente (16,7%), Muito Boa (32,3%), Boa (31,2%), Regular (12,8%), Ruim (4,0%)          |
| 2   | **Checkup**                      | Categórico | "Within the past year", "Within the past 2 years", "Within the past 5 years", "5 or more years ago", "Never"      | **Última Consulta Médica**<br>Tempo desde a última consulta médica de rotina<br>• No último ano (74,4%), Últimos 2 anos (12,5%), Últimos 5 anos (7,0%), 5+ anos (5,4%), Nunca (0,7%) |
| 3   | **Exercise**                     | Binário    | "Yes", "No"                                                                                                       | **Atividade Física**<br>Prática de atividade física ou exercício nos últimos 30 dias (exceto trabalho)<br>• Sim (74,4%), Não (25,6%)                                                 |
| 4   | **Heart_Disease**                | Binário    | "Yes", "No"                                                                                                       | **Doença Cardíaca** ⭐ **VARIÁVEL ALVO**<br>Diagnóstico prévio de doença cardíaca coronária ou infarto do miocárdio<br>• Sim (8,5%), Não (91,5%)                                     |
| 5   | **Skin_Cancer**                  | Binário    | "Yes", "No"                                                                                                       | **Câncer de Pele**<br>Diagnóstico prévio de câncer de pele<br>• Sim (9,4%), Não (90,6%)                                                                                              |
| 6   | **Other_Cancer**                 | Binário    | "Yes", "No"                                                                                                       | **Outros Tipos de Câncer**<br>Diagnóstico prévio de qualquer outro tipo de câncer (exceto pele)<br>• Sim (9,6%), Não (90,4%)                                                         |
| 7   | **Depression**                   | Binário    | "Yes", "No"                                                                                                       | **Depressão**<br>Diagnóstico prévio de transtorno depressivo<br>• Sim (19,1%), Não (80,9%)                                                                                           |
| 8   | **Diabetes**                     | Categórico | "Yes", "No", "No, pre-diabetes or borderline diabetes", "Yes, but female told only during pregnancy"              | **Status de Diabetes**<br>• Não (85,9%), Sim (14,1%)<br>• Inclui pré-diabetes e diabetes gestacional                                                                                 |
| 9   | **Arthritis**                    | Binário    | "Yes", "No"                                                                                                       | **Artrite**<br>Diagnóstico prévio de artrite, artrite reumatoide, gota, lúpus ou fibromialgia<br>• Sim (34,3%), Não (65,7%)                                                          |
| 10  | **Sex**                          | Binário    | "Female", "Male"                                                                                                  | **Sexo**<br>Sexo biológico do respondente<br>• Feminino (52,6%), Masculino (47,4%)                                                                                                   |
| 11  | **Age_Category**                 | Categórico | "18-24", "25-29", "30-34", "35-39", "40-44", "45-49", "50-54", "55-59", "60-64", "65-69", "70-74", "75-79", "80+" | **Categoria de Idade**<br>Faixa etária em grupos de 5 anos<br>• Distribuição: 60-64 (11,4%), 65-69 (11,5%), 70-74 (11,1%), 75-79 (6,5%), 80+ (6,0%)                                  |
| 12  | **Height\_(cm)**                 | Numérico   | 122-229 cm                                                                                                        | **Altura em Centímetros**<br>Altura autorrelatada<br>• Média: 171,2 cm, Mediana: 170 cm                                                                                              |
| 13  | **Weight\_(kg)**                 | Numérico   | 32,66-235,87 kg                                                                                                   | **Peso em Quilogramas**<br>Peso autorrelatado<br>• Média: 84,8 kg, Mediana: 81,7 kg                                                                                                  |
| 14  | **BMI**                          | Numérico   | 13,31-89,1 kg/m²                                                                                                  | **Índice de Massa Corporal**<br>Calculado a partir de altura e peso<br>• Média: 28,9 kg/m², Mediana: 27,8 kg/m²                                                                      |
| 15  | **Smoking_History**              | Binário    | "Yes", "No"                                                                                                       | **Histórico de Tabagismo**<br>Histórico de uso de produtos de tabaco<br>• Sim (42,7%), Não (57,3%)                                                                                   |
| 16  | **Alcohol_Consumption**          | Numérico   | 0-30 drinks                                                                                                       | **Consumo de Álcool**<br>Número de drinks alcoólicos por semana<br>• Média: 5,0 drinks, Mediana: 0 drinks                                                                            |
| 17  | **Fruit_Consumption**            | Numérico   | 0-120 porções                                                                                                     | **Consumo de Frutas**<br>Frequência de consumo de frutas por mês<br>• Média: 28,2 porções, Mediana: 28 porções                                                                       |
| 18  | **Green_Vegetables_Consumption** | Numérico   | 0-120 porções                                                                                                     | **Consumo de Vegetais Verdes**<br>Frequência de consumo de vegetais verdes por mês<br>• Média: 14,5 porções, Mediana: 12 porções                                                     |
| 19  | **FriedPotato_Consumption**      | Numérico   | 0-120 porções                                                                                                     | **Consumo de Batata Frita**<br>Frequência de consumo de batatas fritas por mês<br>• Média: 6,5 porções, Mediana: 4 porções                                                           |

### 2. Textos médicos ou literários relacionados à saúde cardiovascular:

Arquivos no repositório:

- [docs/hipertensao_arterial_sistemica_cab37.txt](docs/hipertensao_arterial_sistemica_cab37.txt) — material técnico sobre HAS.
- [docs/pcdt_hipertensao_arterial_sistemica.txt](docs/pcdt_hipertensao_arterial_sistemica.txt) — PCDT de HAS.
- [docs/mirnas_fisiopatologia_dcv.txt](docs/mirnas_fisiopatologia_dcv.txt) — revisão (miRNAs em doença cardiovascular).
- [docs/gdf15_biomarcador_dcv.txt](docs/gdf15_biomarcador_dcv.txt) — revisão (GDF-15 como biomarcador em DCV).

**Por que esses artigos são relevantes?**  
Cobrem aspectos do cenário **macro** (saúde pública, diretrizes e sintomas/tratamento em HAS) até o cenário **micro** (biomarcadores e mecanismos em DCV), enriquecendo sobremaneira:

- O vocabulário clínico (HAS, sinais, exames, fármacos, condutas);
- O vocabulário biomédico (miRNAs, GDF-15, vias, desfechos).

**Tarefas de NLP (exemplos)**

- **NER/Normalização**: doenças (HAS, DAC, ICC), sinais/sintomas, exames (ECG, MAPA), fármacos (IECA, estatinas), **biomarcadores** (miR-xxx, GDF-15) → mapear para CID-10/SNOMED/LOINC quando aplicável.
- **Classificação de tópicos**: prevenção, diagnóstico, tratamento, seguimento, mecanismos/biomarcadores.
- **Extração de relações**: _biomarcador → condição → prognóstico/tratamento_ (p.ex., “GDF-15 elevado” associado a “pior desfecho em ICC”).
- **Sumarização/QA**: respostas objetivas a partir dos textos de HAS (ex.: metas pressóricas, quando iniciar tratamento).

**Governança e licenças**

- Textos convertidos para **.txt (UTF-8)**; metadados de proveniência no topo de cada arquivo (Título, URL/Fonte, Licença/uso).
- SciELO: utilizar artigos **Acesso Aberto/CC** com **atribuição** no arquivo e no README.
- Sem dados pessoais. Apenas conteúdo público/científico.

### 3. Imagens médicas (exames ou sinais visuais):

Este conjunto de imagens contém registros de ECG coletados usando um dispositivo IoT personalizado equipado com um sensor de ECG. Os dados foram coletados diretamente do corpo humano por meio de eletrodos colocados no peito, capturando a atividade elétrica do coração em tempo real. O conjunto de dados é dividido em três classes: sinais Normais, Anormais e com Histórico de IM (Infarto do Miocárdio), representando uma gama de condições cardíacas.

As imagens estão disponíveis para visualização e download NESTE REPOSITÓRIO, em:

- [assets/imagens_exames_cardiovasculares](assets/imagens_exames_cardiovasculares/)

Ou ainda, para download neste LINK:

- [Google Drive](https://drive.google.com/drive/folders/18-chtpMsnc8khSfv5VKaE4i5B7j_-pTi?usp=drive_link)

---

## 📁 Estrutura de pastas

Dentre os arquivos e pastas presentes na raiz do projeto, definem-se:

- <b>.github</b>: Nesta pasta ficarão os arquivos de configuração específicos do GitHub que ajudam a gerenciar e automatizar processos no repositório.
- <b>assets</b>: aqui estão os arquivos relacionados a elementos não-estruturados deste repositório, como imagens.
- <b>README.md</b>: arquivo que serve como guia e explicação geral sobre o projeto (o mesmo que você está lendo agora).

## 🗃 Histórico de lançamentos

- 0.1.0 - 02/09/2025

## 📋 Licença

<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/by.svg?ref=chooser-v1"><p xmlns:cc="http://creativecommons.org/ns#" xmlns:dct="http://purl.org/dc/terms/"><a property="dct:title" rel="cc:attributionURL" href="https://github.com/agodoi/template">MODELO GIT FIAP</a> por <a rel="cc:attributionURL dct:creator" property="cc:attributionName" href="https://fiap.com.br">Fiap</a> está licenciado sobre <a href="http://creativecommons.org/licenses/by/4.0/?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">Attribution 4.0 International</a>.</p>
