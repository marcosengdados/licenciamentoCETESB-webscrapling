# 🌿 Panorama de Licenciamento CETESB — Pipeline de Sales Intelligence & Lead Scoring

> Leitura consolidada de processos de licenciamento ambiental via Web Scraping, convertida em score de oportunidade, temperatura da carteira e ação comercial recomendada por empreendimento.

---

## 🎯 Visão Geral do Projeto

A prospecção B2B no setor de consultoria e engenharia ambiental enfrenta frequentemente um gargalo operacional: a identificação manual, fragmentada e reativa de demandas regulatórias. Este projeto resolve esse problema por meio de uma arquitetura automatizada de **Extração de Dados (Web Scraping)**, **Engenharia de Dados** e **Sales Intelligence**, que monitora processos administrativos na **CETESB** e os transforma em uma console de priorização comercial acionável (`Leads_Consolidados_CRM`).

O sistema elimina o julgamento humano subjetivo na triagem inicial, calculando o **Score de Oportunidade**, a **Temperatura do Lead** e a **Ação Comercial Recomendada** estritamente a partir da criticidade do status processual, do perfil do empreendimento e do tempo de recência.

---

## 📊 Principais Métricas do Pipeline (Snapshot)

| Indicador (KPI) | Valor Consolidado | Contexto Técnico / Operacional |
| :--- | :---: | :--- |
| 🗂️ **Processos Monitorados** | **263** | Somatório de todos os status processuais extraídos e auditados na varredura |
| 🏢 **Empreendimentos Mapeados** | **74** | Entidades únicas com processo ativo ou histórico relevante identificado na CETESB |
| 🎯 **Score Médio de Oportunidade** | **66,15** | Escala quantitativa de $0$ a $100$ baseada na criticidade regulatória e recência |

---

## 🖥️ Demonstração Visual e Arquitetura Analítica

Abaixo estão as visões consolidadas e os recortes analíticos gerados pelo pipeline, conectando a extração de dados regulatórios à tomada de decisão comercial.

### 1. Visão Executiva Consolidada — Panorama Geral (Página 1)
![Panorama de Licenciamento CETESB - Página 1](Panorama%20Licenciamento%20CETESB%20%28Web%20scrapping%29_page-0001.jpg)
> **Análise da Visão (`Panorama Licenciamento CETESB (Web scrapping)_page-0001.jpg`):** Painel principal do relatório executivo consolidando os indicadores-chave da carteira monitorada ($263$ processos distribuídos em $74$ empreendimentos), distribuição de criticidade, recortes por tipologia de licenciamento (LP, LI, LO, Renovação) e visão macro do funil de prospecção ambiental.

---

### 2. Detalhamento Operacional e Desdobramento de Processos (Página 2)
![Panorama de Licenciamento CETESB - Página 2](Panorama%20Licenciamento%20CETESB%20%28Web%20scrapping%29_page-0002.jpg)
> **Análise da Visão (`Panorama Licenciamento CETESB (Web scrapping)_page-0002.jpg`):** Segunda página do painel analítico voltada ao aprofundamento granular por empreendimento e status administrativo, permitindo cruzar o histórico de tramitação na CETESB com o potencial de conversão em contratos de consultoria técnica.

---

### 3. Temperatura da Carteira e Indicadores-Chave (KPIs)
![Temperatura da Carteira e Indicadores-Chave](Temperatura%20da%20Carteira%20e%20Indicadores-Chave.jpg)
> **Análise do Recorte (`Temperatura da Carteira e Indicadores-Chave.jpg`):** Segmentação termográfica da base de leads (Quente, Morno, Frio) combinada aos KPIs centrais do pipeline. Permite que a diretoria comercial identifique instantaneamente a proporção da carteira que exige abordagem imediata devido a exigências técnicas, indeferimentos ou vencimentos próximos.

---

### 4. Volume de Processos por Segmento Econômico
![Volume por Segmento](Vol.%20por%20segmento.jpg)
> **Análise do Recorte (`Vol. por segmento.jpg`):** Mapeamento da concentração de processos administrativos por setor de atividade e porte do empreendimento. Orienta a alocação de especialistas técnicos (indústria química, infraestrutura, gerenciamento de resíduos, agronegócio) conforme a demanda real observada no órgão ambiental.

---

### 5. Perfil de Contrato e Enquadramento Comercial
![Perfil de Contrato](Perfil%20contrato.png)
> **Análise do Recorte (`Perfil contrato.png`):** Classificação dos empreendimentos segundo o perfil de contratação esperado (projetos pontuais de regularização vs. contratos recorrentes de gestão e acompanhamento ambiental), estruturando a previsibilidade de receita da consultoria.

---

### 6. Pipeline de Serviços Recomendados (Cross-Selling Técnico)
![Pipeline de Serviços Recomendados](Pipeline%20de%20servi%C3%A7os%20recomendados.png)
> **Análise do Recorte (`Pipeline de serviços recomendados.png`):** Motor de recomendação que traduz o status bruto da CETESB em soluções de engenharia comercializáveis (ex.: elaboração de estudos ambientais, atendimento a exigências técnicas, renovação de Licença de Operação, CADRI ou defesa administrativa).

---

### 7. Matriz de Priorização Comercial e Lead Scoring
![Priorização Comercial](priorizacao%20comercial.png)
> **Análise do Recorte (`priorizacao comercial.png`):** Console final de ação para o time de vendas B2B (SDRs e Executivos de Contas), ordenando os empreendimentos pelo Score de Oportunidade (média de $66,15$), status de urgência e próxima ação comercial recomendada.

---

## 🗄️ Arquitetura de Dados e Governança (Repositório)

O repositório foi estruturado para fornecer transparência desde a camada de dados tabulares processados até os artefatos de visualização interativa:

| Arquivo no Repositório | Camada | Descrição Técnica e Papel no Pipeline |
| :--- | :---: | :--- |
| `dicionario_dados.csv` | **Governança** | Documentação de metadados, tipagem, regras de negócio e semântica de cada coluna gerada no pipeline. |
| `analise_empreendimento.csv` | **Camada Analítica** | Visão agregada por entidade empresarial ($74$ empreendimentos), contendo score consolidado e classificação comercial. |
| `analise_status.csv` | **Camada Analítica** | Consolidação volumétrica e qualitativa por etapa do fluxo regulatório na CETESB ($263$ processos). |
| `analise_status_empreendimento.csv` | **Camada Analítica** | Tabela fato relacionando cada empreendimento aos seus respectivos status processuais e tempos de recência. |
| `top_100_empreendimentos.csv` | **Sales Intelligence** | Ranking priorizado de contas de maior potencial para importação direta em ferramentas de CRM. |
| `index.html` | **Front-End / Web** | Console interativa em HTML para visualização rápida e compartilhamento executivo dos resultados. |
| `Panorama Licenciamento CETESB (Web scrapping).pbit` | **Business Intelligence** | Template oficial do Power BI contendo a modelagem de dados, medidas DAX e visuais configurados. |
| `Panorama Licenciamento CETESB (Web scrapping).pdf` | **Relatório Executivo** | Versão estática de alta resolução para distribuição em reuniões de diretoria e apresentações comerciais. |

---

## ⚙️ Metodologia de Cálculo do Lead Scoring

A pontuação de cada oportunidade segue um modelo determinístico auditável:

$$\text{Score de Oportunidade} = f(\text{Criticidade do Status}, \text{Recência da Movimentação}, \text{Volume de Processos})$$

1. **Extração Automatizada (Web Scraping):** Coleta estruturada dos registros públicos de licenciamento ambiental junto ao portal da CETESB.
2. **Saneamento e Padronização:** Limpeza de strings, unificação de razões sociais/empreendimentos e catalogação documentada em `dicionario_dados.csv`.
3. **Atribuição de Score e Temperatura:** Classificação objetiva de $0$ a $100$ para eliminar viés na prospecção.
4. **Prescrição Comercial:** Associação automática de cada faixa de status a um serviço técnico específico do portfólio da consultoria.

---

## 🚀 Como Utilizar os Artefatos deste Repositório

1. **Exploração Rápida dos Dados:** Consulte `dicionario_dados.csv` para compreender o schema e explore `top_100_empreendimentos.csv` para visualizar a saída pronta para o CRM.
2. **Visualização no Power BI:** Baixe o arquivo `Panorama Licenciamento CETESB (Web scrapping).pbit`, abra no **Power BI Desktop** e aponte a origem de dados para os arquivos `.csv` locais deste repositório.
3. **Visualização Web / Executiva:** Abra o arquivo `index.html` em qualquer navegador ou consulte o relatório consolidado em `Panorama Licenciamento CETESB (Web scrapping).pdf`.
