# CardioIA – Fase 1: Batimentos de Dados

Este repositório faz parte do projeto **CardioIA**, cujo objetivo é simular um ecossistema de cardiologia inteligente utilizando técnicas de **Inteligência Artificial aplicadas à área da saúde**.

Nesta primeira fase do projeto foi realizado o levantamento e organização de diferentes tipos de dados que poderão futuramente alimentar algoritmos de IA voltados à análise e predição de doenças cardiovasculares.

Os dados coletados incluem:

* Dados numéricos clínicos
* Dados textuais médicos

Esses dados servirão como base para o desenvolvimento das próximas fases do projeto.

---

# Parte 1 – Dados Numéricos (IoT)

Nesta etapa foi utilizado um dataset contendo **informações clínicas de pacientes avaliados quanto à presença de doenças cardíacas**.

O dataset foi obtido do **UCI Machine Learning Repository**, um dos repositórios acadêmicos mais utilizados em pesquisas de **Machine Learning e Data Science**.

Os dados foram coletados utilizando a biblioteca Python **ucimlrepo**.

Link para acesso ao dataset completo:

https://drive.google.com/file/d/1-xJZd8n4U8sgl-1rGVsMl-QthgCIOMo_/view?usp=drive_link

---

# Estrutura do Dataset

O arquivo principal utilizado neste projeto é:

```
pacientes_cardiacos.csv
```

Cada linha representa um **paciente**, enquanto cada coluna representa uma **variável clínica relevante para análise cardiovascular**.

O dataset possui **mais de 300 registros**, atendendo ao requisito mínimo de 100 linhas solicitado na atividade.

---

# Descrição das Variáveis

| Variável | Significado            | Descrição                                                |
| -------- | ---------------------- | -------------------------------------------------------- |
| age      | Idade                  | Idade do paciente em anos                                |
| sex      | Sexo                   | Sexo biológico do paciente (1 = masculino, 0 = feminino) |
| cp       | Chest Pain Type        | Tipo de dor no peito relatada pelo paciente              |
| trestbps | Resting Blood Pressure | Pressão arterial em repouso (mmHg)                       |
| chol     | Cholesterol            | Nível de colesterol no sangue (mg/dl)                    |
| fbs      | Fasting Blood Sugar    | Açúcar no sangue em jejum                                |
| restecg  | Resting ECG            | Resultado do eletrocardiograma em repouso                |
| thalach  | Maximum Heart Rate     | Frequência cardíaca máxima atingida                      |
| exang    | Exercise Angina        | Presença de dor no peito durante exercício               |
| oldpeak  | ST Depression          | Alteração observada no ECG após esforço                  |
| slope    | ST Segment Slope       | Inclinação do segmento ST no eletrocardiograma           |
| ca       | Number of Vessels      | Número de vasos sanguíneos principais afetados           |
| thal     | Thalassemia Test       | Resultado de exame cardíaco específico                   |
| target   | Diagnóstico            | Indica presença ou ausência de doença cardíaca           |

---

# Interpretação de Algumas Variáveis

### Tipo de dor no peito (cp)

| Valor | Significado                    |
| ----- | ------------------------------ |
| 0     | Angina típica                  |
| 1     | Angina atípica                 |
| 2     | Dor não relacionada ao coração |
| 3     | Assintomático                  |

### Angina induzida por exercício (exang)

| Valor | Significado |
| ----- | ----------- |
| 0     | Não         |
| 1     | Sim         |

### Açúcar no sangue em jejum (fbs)

| Valor | Significado                   |
| ----- | ----------------------------- |
| 0     | Normal                        |
| 1     | Elevado (maior que 120 mg/dl) |

### Diagnóstico de doença cardíaca (target)

| Valor | Significado                 |
| ----- | --------------------------- |
| 0     | Ausência de doença cardíaca |
| 1     | Presença de doença cardíaca |

---

# Variáveis Clinicamente Relevantes

Algumas variáveis são especialmente importantes para análise em projetos de **Inteligência Artificial aplicada à saúde**.

**Idade (age)**
O risco de doenças cardiovasculares aumenta com o envelhecimento, tornando essa variável fundamental para modelos preditivos.

**Pressão arterial em repouso (trestbps)**
A hipertensão é um dos principais fatores de risco para infarto e acidente vascular cerebral (AVC).

**Colesterol (chol)**
Níveis elevados de colesterol estão associados ao acúmulo de placas nas artérias, podendo causar obstrução do fluxo sanguíneo.

**Frequência cardíaca máxima (thalach)**
Pode indicar a capacidade cardiovascular do paciente e revelar possíveis anomalias cardíacas.

**Tipo de dor no peito (cp)**
A dor no peito é um dos sintomas mais clássicos de doenças coronarianas e pode indicar diferentes condições cardíacas.

---

# Importância para Inteligência Artificial

Esses dados podem ser utilizados para o treinamento de **modelos de Machine Learning capazes de prever o risco de doenças cardíacas**, identificar padrões clínicos e auxiliar profissionais da saúde no processo de diagnóstico.

A utilização de datasets clínicos estruturados é fundamental para o desenvolvimento de **sistemas inteligentes aplicados à área médica**, como o projeto **CardioIA**, que busca integrar análise de dados, automação e suporte à decisão clínica.

---

# Parte 2 – Dados Textuais (NLP)

Também foram coletados **textos médicos relacionados a doenças cardiovasculares**, sintomas de infarto e fatores de risco cardíacos.

Esses textos foram obtidos de **fontes confiáveis de saúde pública e literatura médica**, incluindo materiais informativos sobre:

* insuficiência cardíaca
* infarto do miocárdio
* fatores de risco cardiovasculares
* prevenção de doenças cardíacas

Os arquivos estão disponíveis na pasta:

```
docs/
```

---

# Aplicações de NLP

Esses textos podem ser utilizados em projetos de Inteligência Artificial utilizando técnicas de **Processamento de Linguagem Natural (NLP)**.

Algumas aplicações possíveis incluem:

* Extração automática de sintomas (ex: dor no peito, falta de ar)
* Identificação de fatores de risco (ex: hipertensão, colesterol alto, obesidade)
* Classificação de doenças cardiovasculares
* Análise de literatura médica

Essas técnicas permitem que sistemas de IA analisem **relatórios clínicos, prontuários médicos e artigos científicos**, auxiliando no diagnóstico e na tomada de decisões médicas.
