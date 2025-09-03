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

#### Dados numéricos:

- TBD

#### Textos médicos ou literários relacionados à saúde cardiovascular:

- TBD

#### Imagens médicas (exames ou sinais visuais):

Nova tabela adicionada com os seguintes campos, abaixo explicados:

## Parte 2 — Dados Textuais (NLP) — Conjunto (PT-BR)

Arquivos no repositório:
## Parte 2 — Dados Textuais (NLP) — Conjunto (PT-BR)

Arquivos no repositório:
- [docs/hipertensao_arterial_sistemica_cab37.txt](docs/hipertensao_arterial_sistemica_cab37.txt) — material técnico sobre HAS.
- [docs/pcdt_hipertensao_arterial_sistemica.txt](docs/pcdt_hipertensao_arterial_sistemica.txt) — PCDT de HAS.
- [docs/mirnas_fisiopatologia_dcv.txt](docs/mirnas_fisiopatologia_dcv.txt) — revisão (miRNAs em doença cardiovascular).
- [docs/gdf15_biomarcador_dcv.txt](docs/gdf15_biomarcador_dcv.txt) — revisão (GDF-15 como biomarcador em DCV).


**Por que estes 4 juntos?**  
Cobrem do **macro** (saúde pública, diretrizes e sintomas/tratamento em HAS) ao **micro** (biomarcadores e mecanismos em DCV). Isso enriquece:
- o vocabulário clínico (HAS, sinais, exames, fármacos, condutas);
- o vocabulário biomédico (miRNAs, GDF-15, vias, desfechos).

**Tarefas de NLP (exemplos)**
- **NER/Normalização**: doenças (HAS, DAC, ICC), sinais/sintomas, exames (ECG, MAPA), fármacos (IECA, estatinas), **biomarcadores** (miR-xxx, GDF-15) → mapear para CID-10/SNOMED/LOINC quando aplicável.
- **Classificação de tópicos**: prevenção, diagnóstico, tratamento, seguimento, mecanismos/biomarcadores.
- **Extração de relações**: *biomarcador → condição → prognóstico/tratamento* (p.ex., “GDF-15 elevado” associado a “pior desfecho em ICC”).
- **Sumarização/QA**: respostas objetivas a partir dos textos de HAS (ex.: metas pressóricas, quando iniciar tratamento).

**Governança e licenças**
- Textos convertidos para **.txt (UTF-8)**; metadados de proveniência no topo de cada arquivo (Título, URL/Fonte, Licença/uso).  
- SciELO: utilizar artigos **Acesso Aberto/CC** com **atribuição** no arquivo e no README.  
- Sem dados pessoais. Apenas conteúdo público/científico.


## 📁 Estrutura de pastas

Dentre os arquivos e pastas presentes na raiz do projeto, definem-se:

- <b>.github</b>: Nesta pasta ficarão os arquivos de configuração específicos do GitHub que ajudam a gerenciar e automatizar processos no repositório.
- <b>assets</b>: aqui estão os arquivos relacionados a elementos não-estruturados deste repositório, como imagens.
- <b>README.md</b>: arquivo que serve como guia e explicação geral sobre o projeto (o mesmo que você está lendo agora).

## 🗃 Histórico de lançamentos

- 0.1.0 - 02/09/2025

## 📋 Licença

<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/by.svg?ref=chooser-v1"><p xmlns:cc="http://creativecommons.org/ns#" xmlns:dct="http://purl.org/dc/terms/"><a property="dct:title" rel="cc:attributionURL" href="https://github.com/agodoi/template">MODELO GIT FIAP</a> por <a rel="cc:attributionURL dct:creator" property="cc:attributionName" href="https://fiap.com.br">Fiap</a> está licenciado sobre <a href="http://creativecommons.org/licenses/by/4.0/?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">Attribution 4.0 International</a>.</p>
