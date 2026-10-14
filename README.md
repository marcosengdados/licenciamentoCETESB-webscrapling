## 📈 Business Intelligence & Revenue Operations (RevOps)

Mais do que um painel de visualização, esta camada de BI atua como o **motor de inteligência comercial (Sales Intelligence)** da operação. Desenvolvido em Power BI com modelagem *Star Schema* e governança de dados estrita, o painel traduz o complexo cenário regulatório paulista em ações de vendas de altíssima conversão.

Nesse projeto a analise se fundamenta em não olhar para "processos ambientais", e sim para **oportunidades**. Abaixo, o desdobramento estratégico de cada visão do nosso pipeline:

<div align="center">

### 1. Portfólio e Market Share
<img src="Panorama%20Licenciamento%20CETESB%20%28Web%20scrapping%29_page-0001.jpg" width="850" style="border-radius: 8px; border: 2px solid #1b4332;">
<p align="left">
<i><b>Impacto Executivo & ROI:</b> Nossa varredura capturou <b>263 processos ativos distribuídos em 74 contas (CNPJs)</b>. A proporção de <b>3,5 processos por cliente</b> é o nosso indicador-chave de <b>Upsell/Cross-sell</b>. Se o dashboard aponta um gargalo sistêmico em "Renovações de LO" no estado, nós pivotamos a estratégia de marketing e as metas do trimestre para atacar especificamente essa dor. É a visão macro que direciona o esforço da companhia.</i>
</p>

### 2. Visão Tática (Deal Desk): Desdobramento de Contas Estratégicas (Key Accounts)
<img src="Panorama%20Licenciamento%20CETESB%20%28Web%20scrapping%29_page-0002.jpg" width="850" style="border-radius: 8px; border: 2px solid #1b4332;">
<p align="left">
<i><b>Impacto Executivo & ROI:</b> Esta é a tela que reduz nosso Custo de Aquisição de Clientes (CAC) e encurta o Ciclo de Vendas. O Executivo de Contas não faz "cold calls" genéricas. Ao isolar um CNPJ, o gráfico entrega uma assimetria de informação letal: sabemos exatamente qual licença está travada, há quantos dias, e qual documento falta. A abordagem comercial deixa de ser "oferecer consultoria" e passa a ser <b>"resolver o passivo milionário da fábrica que está parado na mesa do analista"</b>.</i>
</p>

</div>

---

### 🔍 Unidades de Inteligência Comercial (Módulos do Dashboard)

<details open>
<summary><b>🔥 1. Pipeline Velocity: Termômetro da Carteira</b></summary>
<br>
<div align="center">
<img src="Temperatura%20da%20Carteira%20e%20Indicadores-Chave.jpg" width="800">
</div>
<br>
<b>Estratégia de Conversão:</b> Gestão rigorosa de SLA comercial. Os <i>Leads Quentes</i> (Score > 80) representam <b>receita de curtíssimo prazo</b> — licenças indeferidas, embargos ou vencimentos em 30 dias que exigem "Tropa de Choque" imediata. A proporção de <i>Leads Mornos</i> garante o nosso <i>backlog</i> (pipeline de Q3/Q4). Se a proporção de leads frios cresce, sabemos que precisamos recalibrar os filtros do Web Scraper para buscar contas mais qualificadas.
</details>

<details open>
<summary><b>🏭 2. Total Addressable Market (TAM): Concentração Setorial</b></summary>
<br>
<div align="center">
<img src="Vol.%20por%20segmento.jpg" width="800">
</div>
<br>
<b>Estratégia de Conversão:</b> Direcionamento de <i>Headcount</i> técnico. Se o gráfico revela que <b>45% da demanda regulatória latente está na Indústria Química e em Gestão de Resíduos</b>, é para lá que direcionamos nossos engenheiros seniores nas reuniões de <i>closing</i> (fechamento). Não desperdiçamos recursos de prospecção em setores (CNAEs) onde o volume de processos é irrisório.
</details>

<details open>
<summary><b>💼 3. Motor de SDR: Matriz de Priorização B2B</b></summary>
<br>
<div align="center">
<img src="priorizacao%20comercial.png" width="800">
</div>
<br>
<b>Estratégia de Conversão:</b> Eliminação total de viés humano. O <b>Score Médio de 66,15</b> normaliza a urgência. O time de pré-vendas (SDRs) atua estritamente ordenando a tabela de cima para baixo. O cruzamento visual de <b>Criticidade Regulatória vs. Porte Financeiro da Empresa</b> garante que o tempo valioso da equipe comercial seja focado nos <i>Enterprise Deals</i> (tickets médios mais altos), maximizando o Retorno sobre o Tempo Investido.
</details>

<details>
<summary><b>🤝 4. Product-Market Fit Dinâmico: Sugestão de Portfólio</b></summary>
<br>
<div align="center">
<img src="Pipeline%20de%20servi%C3%A7os%20recomendados.png" width="800">
</div>
<br>
<b>Estratégia de Conversão:</b> Tradução automática do "problema" no "SKU" correto. O algoritmo lê um status burocrático obscuro (ex: <i>"Aguardando manifestação técnica de terceiros - DAEE"</i>) e orienta o time de vendas: <i>"Ofereça o serviço de Estudo de Outorga"</i>. Isso escala a inteligência comercial, permitindo que vendedores júniores negociem com a precisão de diretores técnicos.
</details>

<details>
<summary><b>📊 5. Previsibilidade Financeira: MRR vs. One-Off</b></summary>
<br>
<div align="center">
<img src="Perfil%20contrato.png" width="800">
</div>
<br>
<b>Estratégia de Conversão:</b> Modelagem de fluxo de caixa preditivo. Entender a proporção da carteira extraída divide o foco estratégico: empresas com perfil <b>One-Off</b> trazem injeção rápida de caixa (ex: licença prévia pontual), enquanto empresas com múltiplas plantas e dezenas de licenças são direcionadas para o funil de <b>MRR (Monthly Recurring Revenue)</b>, garantindo contratos anuais de terceirização do departamento ambiental.
</details>
<div align="center">
  <br>
  <b>Pronto para rodar no seu CRM?</b> Baixe o artefato <code>top_100_empreendimentos.csv</code> ou abra o <code>.pbit</code> no Power BI Desktop para conectar às suas próprias fontes de dados.
</div>
