<div align="center">

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:081c15,50:1b4332,100:2d6a4f&height=220&section=header&text=Licenciamento%20CETESB&fontSize=46&fontColor=d8f3dc&animation=fadeIn&fontAlignY=35&desc=Motor%20de%20Prioriza%C3%A7%C3%A3o%20e%20Intelig%C3%AAncia%20Comercial&descAlignY=60&descSize=18&descColor=b7e4c7"/>

<img src="https://img.shields.io/badge/Python-081c15?style=for-the-badge&logo=python&logoColor=d8f3dc&labelColor=1b4332"/>
<img src="https://img.shields.io/badge/Playwright-081c15?style=for-the-badge&logo=playwright&logoColor=d8f3dc&labelColor=1b4332"/>
<img src="https://img.shields.io/badge/Power_BI-081c15?style=for-the-badge&logo=powerbi&logoColor=d8f3dc&labelColor=1b4332"/>
<img src="https://img.shields.io/badge/DAX-081c15?style=for-the-badge&logo=microsoft&logoColor=d8f3dc&labelColor=1b4332"/>
<img src="https://img.shields.io/badge/Engenharia_de_Dados-081c15?style=for-the-badge&logo=databricks&logoColor=d8f3dc&labelColor=1b4332"/>

<br>

> Automação da triagem de processos ambientais para otimizar a abordagem comercial e reduzir o tempo de resposta do setor.

</div>

---

## 🎯 Visão Geral da Solução

O monitoramento manual de demandas regulatórias gera atrasos na identificação de oportunidades e consome tempo operacional da equipe. Para resolver esse gargalo, desenvolvemos um pipeline automatizado que varre o portal da **CETESB**, extrai os status processuais atualizados e os converte em um painel interativo de priorização comercial.

O sistema elimina a necessidade de triagem manual diária. Através de um algoritmo interno, cruzamos a criticidade do status ambiental com o perfil do empreendimento, gerando um **Score de Oportunidade** que indica para a equipe comercial exatamente quem contatar, qual é a urgência e qual serviço oferecer.

---

## ⚡ Volumetria e Impacto Operacional

| Indicador | Volume Mapeado | Valor Prático para o Setor |
| :--- | :---: | :--- |
| 🗂️ **Processos** | **263** | Passivos ou trâmites ativos acompanhados de forma 100% automatizada. |
| 🏢 **Empreendimentos** | **74** | Contas (CNPJs) com necessidades regulatórias identificadas na base. |
| 🎯 **Score Médio** | **66,15** | Grau de urgência da carteira, orientando o esforço de contato da semana. |

---

## 🖥️ Painéis de Inteligência e Aplicação Prática

A interface de Business Intelligence foi desenhada para dar suporte rápido à tomada de decisão da coordenação e guiar o dia a dia da equipe de pré-vendas/SDRs.

<div align="center">

### 1. Panorama Consolidado da Carteira
<img src="Panorama%20Licenciamento%20CETESB%20%28Web%20scrapping%29_page-0001.jpg" width="850" style="border-radius: 8px; border: 2px solid #1b4332;">
<p align="left">
<i><b>Uso na Coordenação:</b> Permite visualizar o "tamanho do problema" no estado. Se notamos um pico de <b>Renovações de LO</b> travadas, podemos orientar a equipe a focar o discurso da semana nesse serviço específico, alinhando a capacidade técnica interna com a demanda imediata do mercado.</i>
</p>

### 2. Aprofundamento por Empreendimento (Raio-X)
<img src="Panorama%20Licenciamento%20CETESB%20%28Web%20scrapping%29_page-0002.jpg" width="850" style="border-radius: 8px; border: 2px solid #1b4332;">
<p align="left">
<i><b>Uso na Abordagem Comercial:</b> É a ferramenta de preparo da equipe. Antes de ligar para o cliente, o analista isola o CNPJ e entende o cenário completo: descobre se o gargalo é uma <b>Exigência Técnica pendente há 45 dias</b> ou um documento faltante. A abordagem deixa de ser genérica e passa a ser uma oferta de solução imediata para um passivo real.</i>
</p>

</div>

---

### 🔍 Detalhamento dos Módulos de Apoio

<details open>
<summary><b>🔥 1. Temperatura e Matriz de Urgência</b></summary>
<br>
<div align="center">
<img src="Temperatura%20da%20Carteira%20e%20Indicadores-Chave.jpg" width="800">
</div>
<br>
O sistema quantifica o risco temporal. Leads <b>Quentes</b> destacam empresas com prazos vencendo rapidamente ou indeferimentos recentes — são os contatos prioritários do dia para garantir conversões rápidas. Leads <b>Mornos</b> alimentam a fila de cadência para os próximos meses.
</details>

<details open>
<summary><b>🏭 2. Concentração Setorial (Alocação de Equipe)</b></summary>
<br>
<div align="center">
<img src="Vol.%20por%20segmento.jpg" width="800">
</div>
<br>
Mapeia a origem da demanda por setor (CNAE). Se os dados mostram que a maior fatia de processos travados está na <b>Indústria Química ou Gestão de Resíduos</b>, a coordenação sabe que precisará envolver os engenheiros especialistas nestes temas (ex: peritos em CADRI) nas reuniões comerciais mais importantes da semana.
</details>

<details open>
<summary><b>💼 3. O Sistema P1 a P4: Automação da Rotina de Vendas</b></summary>
<br>
<div align="center">
<img src="priorizacao%20comercial.png" width="800">
</div>
<br>
Para eliminar o viés da equipe na hora de escolher "para quem ligar hoje", o algoritmo mastiga a base e classifica os leads em 4 níveis de prioridade de atuação (Matriz P1 a P4):
<br><br>
<ul>
  <li>🚨 <b>P1 (Urgência Máxima):</b> Prazos estourando ou exigências críticas em contas de alto ticket. Exige ligação imediata (D+0) pelo Executivo de Contas Sênior.</li>
  <li>⚠️ <b>P2 (Alta Prioridade):</b> Vencimentos próximos (ex: LO expirando em 60 dias) com alta chance de conversão. Abordagem ativa do SDR para estruturar a proposta técnica com antecedência.</li>
  <li>📅 <b>P3 (Prioridade Média):</b> Processos em andamento normal no órgão. O cliente entra em uma cadência de acompanhamento quinzenal (Follow-up) para criar relacionamento.</li>
  <li>💤 <b>P4 (Baixa Prioridade / Nutrição):</b> Processos paralisados há muito tempo, inativos ou tickets muito baixos. Direcionados automaticamente para campanhas de e-mail marketing, poupando o telefone da equipe.</li>
</ul>
</details>

<details>
<summary><b>🤝 4. Sugestão Automática de Serviços</b></summary>
<br>
<div align="center">
<img src="Pipeline%20de%20servi%C3%A7os%20recomendados.png" width="800">
</div>
<br>
Uma matriz interna que traduz o status burocrático da CETESB para o nosso catálogo. Se o status é <i>"Aguardando manifestação do DAEE"</i>, o painel já sugere oferecer <i>"Estudo de Outorga"</i>. Isso acelera a formulação de propostas e ajuda membros mais novos da equipe a acertarem a oferta técnica.
</details>

<details>
<summary><b>📊 5. Perfil de Contrato (Gestão do Funil)</b></summary>
<br>
<div align="center">
<img src="Perfil%20contrato.png" width="800">
</div>
<br>
Classifica a base extraída para equilibrar o tipo de prospecção: mostra quantas empresas têm perfil para serviços pontuais rápidos (injeção de caixa a curto prazo) e quantas justificam o esforço para fechar contratos de gestão contínua e terceirização ambiental (receita recorrente).
</details>

---

## 🗄️ Estrutura e Governança do Projeto

O repositório está organizado para garantir que a coordenação e a equipe técnica possam auditar ou adaptar o pipeline conforme novas necessidades do setor:

| Artefato | Função na Operação |
| :--- | :--- |
| 📖 `dicionario_dados.csv` | Documentação das regras de negócio aplicadas na limpeza dos dados. |
| 🏭 `analise_empreendimento.csv` | Base consolidada por CNPJ com as pontuações finais para importação. |
| 📜 `analise_status.csv` | Volumetria de processos por etapa do fluxo na CETESB. |
| 🏆 `top_100_empreendimentos.csv` | **Planilha final higienizada, pronta para a equipe de vendas / importação no CRM.** |
| 📊 `Panorama Licenciamento CETESB.pbit` | Template do Power BI para atualização recorrente com novos dados. |
| 🌐 `index.html` | Interface web leve para visualização rápida dos números pelo time. |
