# 🌿 Panorama de Licenciamento CETESB — Pipeline de Sales Intelligence & Lead Scoring

> **Leitura consolidada de processos de licenciamento ambiental via Web Scraping, convertida em score de oportunidade e ação comercial recomendada por empreendimento.**[cite: 1]

---

## 🎯 Visão Geral do Projeto

A prospecção B2B no setor de consultoria e engenharia ambiental enfrenta frequentemente um gargalo operacional: a identificação manual e reativa de demandas regulatórias. Este projeto resolve esse problema através de uma arquitetura automatizada de **Extração de Dados (Web Scraping)** e **Engenharia de Dados**, que monitora processos administrativos na **CETESB** e os transforma numa consola de priorização comercial acionável (`Leads_Consolidados_CRM`)[cite: 1, 2].

O sistema elimina o julgamento humano subjetivo na triagem inicial, calculando o **Score**, a **Temperatura** e a **Ação Comercial** estritamente a partir do status processual e do tempo de recência[cite: 2].

---

## 📊 Principais Métricas do Pipeline (Snapshot)

| Indicador (KPI) | Valor Consolidado | Contexto Técnico / Operacional |
| :--- | :--- | :--- |
| 📁 **Processos Monitorados** | **263**[cite: 1, 4] | Somatório de todos os status processuais extraídos na varredura[cite: 1]. |
| 🏢 **Empreendimentos Mapeados** | **74**[cite: 1, 4] | Entidades únicas com processo ativo identificado na CETESB[cite: 1]. |
| 🎯 **Score Médio de Oportunidade** | **66.15**[cite: 1, 4] | Escala quantitativa de 0 a 100 baseada na criticidade regulatória[cite: 1, 2]. |
| 🔥 **Leads Quentes Prioritários** | **39 (53%)**[cite: 1, 4] | Fração da carteira com tração imediata de abordagem comercial[cite: 1]. |

---

## ⚙️ Arquitetura de Inteligência e Regras de Negócio

O pipeline processa os dados brutos e aplica três camadas analíticas para alimentar a equipa comercial:

1. **Higienização e Consolidação (`Leads_Consolidados_CRM`):** Agrupamento de múltiplos processos por CNPJ/Empreendimento, mantendo a rastreabilidade da data de referência (ex.: `20/09/2026`)[cite: 1].
2. **Algoritmo de Lead Scoring & Temperatura:**
   * Avalia o **Status Processual** (ex.: *"Aguardando documentos"* ou *"Aguardando providências do interessado"*) em conjunto com a **Recência** (dias corridos, variando na amostra crítica entre 241 e 461 dias)[cite: 2].
   * Segmenta a carteira em quatro níveis de prioridade operacional: **P1. Urgente**, **P2. Alta**, **P3. Média** e **P4. Renovação**[cite: 2].
3. **Motor de Recomendação de Serviços (*Recommendation Engine*):** Cruza a exigência técnica do órgão ambiental com o portfólio de engenharia, classificando automaticamente o **Perfil de Contrato** entre receita **Pontual** e **Recorrente**[cite: 2].

---

## 📈 Análise das Visualizações e Resultados

### 1️⃣ Volume por Segmento de Atuação
*(Insira aqui a Imagem 1 gerada anteriormente)*

Mapeamento da densidade de mercado por setor industrial (nº de empreendimentos), permitindo alocar especialistas técnicos conforme a vocação da carteira[cite: 1, 3]:

* 🧪 **Química e Farmacêutica:** 39 empreendimentos (Líder em volume de processos)[cite: 1, 3]
* 🏭 **Alimentos e Bebidas:** 32 empreendimentos[cite: 1, 3]
* ⛽ **Combustíveis / Auto Postos:** 27 empreendimentos[cite: 1, 3]
* ⚙️ **Siderurgia e Metalurgia:** 24 empreendimentos[cite: 1, 3]
* 📡 **Infraestrutura e Telecomunicações:** 23 empreendimentos[cite: 1, 3]
* ♻️ **Gestão de Resíduos e Meio Ambiente:** 19 empreendimentos[cite: 1, 3]
* 🌱 **Agronegócio e Sucroalcooleiro:** 17 empreendimentos[cite: 1, 3]
* 🏗️ **Construção Civil e Loteamentos:** 17 empreendimentos[cite: 1, 3]

---

### 2️⃣ Temperatura da Carteira e Qualificação
*(Insira aqui a Imagem 2 gerada anteriormente)*

Distribuição dos **74 empreendimentos** segundo o estágio de maturação da oportunidade comercial[cite: 1, 4]:

* 🟢 **Ativo:** 30 leads (**40.54%**) — Processos em andamento regular com oportunidades de acompanhamento e renovação[cite: 1, 4].
* 🔴 **Quente:** 29 leads (**39.19%**) — Empreendimentos com pendências técnicas diretas ou exigências ativas no órgão ambiental[cite: 1, 2, 4].
* 🟡 **Morno:** 10 leads (**13.51%**) — Demandas de médio prazo para fluxo de nutrição[cite: 1, 4].
* 🔵 **Frio:** 5 leads (**6.76%**) — Baixa prioridade imediata, mantidos em monitoramento automatizado[cite: 1, 4].

#### 🏆 Top Empreendimentos Priorizados (Amostra P1/Alta Criticidade)
Exemplos reais extraídos pela consola demonstrando a conversão de gargalos processuais em inteligência de vendas[cite: 2]:
* **AÇUCAREIRA QUATÁ S.A.** | Status: *Aguardando providências do interessado* | **Score: 91** (Quente) | Recência: 243 dias ➡️ *Serviço: Plano de Aplicação de Vinhaça e Outorga de Captação*[cite: 2].
* **AKZO NOBEL LTDA** | Status: *Aguardando providências do interessado* | **Score: 91** (Quente) | Recência: 245 dias ➡️ *Serviço: Estudo de Análise de Risco (EAR) e CADRI*[cite: 2].
* **3M DO BRASIL LTDA** | Status: *Aguardando providências do interessado* | **Score: 90** (Quente) | Recência: 312 dias ➡️ *Serviço: Estudo de Análise de Risco (EAR) e CADRI*[cite: 2].
* **ADUBOS REAL S/A** & **AGROTERENAS S.A.** | Status: *Aguardando documentos* | **Score: 89** (Quente) | Recência: 241 e 396 dias ➡️ *Serviço: Plano de Aplicação de Vinhaça e Outorga de Captação*[cite: 2].

---

### 3️⃣ Pipeline de Serviços Recomendados & Mix de Receita
*(Insira aqui a Imagem 3 gerada anteriormente)*

Tradução direta dos status da CETESB em oportunidades de negócio estruturadas por linha de serviço e previsibilidade financeira[cite: 2, 5]:

**Demanda Mapeada por Tipologia Técnica (Nº de Leads):**
* 📅 **Contrato de Assessoria Ambiental Mensal:** 14 leads[cite: 2, 5]
* 🚨 **Atendimento a Notificações CETESB:** 10 leads[cite: 2, 5]
* 💧 **Adequação de Efluentes Industriais e Outorga DAEE:** 6 leads[cite: 2, 5]
* 🌾 **Plano de Aplicação de Vinhaça e Outorga de Captação:** 6 leads[cite: 2, 5]
* 🧱 **PGRCC e Gestão Ambiental de Canteiro:** 5 leads[cite: 2, 5]
* ⚠️ **Estudo de Análise de Risco (EAR) e CADRI:** 5 leads[cite: 2, 5]
* 📋 **Auditoria de Condicionantes Ambientais:** 5 leads[cite: 2, 5]
* 🧪 **Investigação SASC e Ensaio de Estanqueidade (CONAMA 273):** 4 leads[cite: 2, 5]
* 🚛 **Gestão de MTR/SIGOR e Destinação de Resíduos:** 4 leads[cite: 2, 5]
* ✅ **Auditoria de Conformidade e Renovação de LO:** 4 leads[cite: 2, 5]

**Mix de Receita Potencial (Perfil de Contrato):**
* 🎯 **Projetos Pontuais:** **36 oportunidades** (Foco em geração de caixa rápido e entrada na conta)[cite: 2, 5].
* 🔄 **Contratos Recorrentes (181 a 365 dias):** **26 oportunidades** (Foco em retenção e previsibilidade de receita)[cite: 2, 5].
* 🛡️ **Contratos de Longo Prazo (+365 dias):** **2 oportunidades** (Foco em contas estratégicas de longo ciclo)[cite: 2, 5].

---

## 🛠️ Stack Tecnológica & Metodologia

* **Data Acquisition:** Automação de coleta (Web Scraping) em portais públicos de licenciamento ambiental (CETESB)[cite: 1, 2].
* **Data Wrangling & CRM Integration:** Estruturação relacional na base `Leads_Consolidados_CRM`, com normalização de status processuais e cálculo de recência temporal[cite: 1, 2].
* **Business Intelligence & DataViz:** Consola analítica interativa para ordenação multicritério (Prioridade, Score, Temperatura e Tipologia de Serviço)[cite: 1, 2].

---
*📌 **Nota Metodológica:** O score, a temperatura e a ação comercial recomendada são calculados de forma 100% determinística a partir do status processual público, garantindo escalabilidade e imparcialidade na priorização da equipa de vendas[cite: 2].*
