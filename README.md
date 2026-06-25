#  Dashboard de Análise de Compras - [Empresa Fictícia]

Este repositório contém a estrutura, o modelo de dados e as configurações do **Dashboard de Compras**, desenvolvido para fornecer uma visão analítica e estratégica sobre a relação de suprimentos, gastos e fornecedores de uma empresa fictícia em um determinado período de tempo[cite: 4].

O objetivo deste relatório é capacitar os gestores com insights visuais rápidos sobre o volume de compras, permitindo a otimização de custos, identificação de sazonalidade e avaliação de parceiros comerciais.

---

## Estrutura e Arquitetura do Projeto

O projeto foi construído utilizando as melhores práticas de business intelligence, tendo sua infraestrutura dividida nos seguintes componentes essenciais[cite: 4]:

* **Modelo de Dados (`DataModel`)**: Estrutura robusta contendo tabelas fato (registro de compras) e tabelas dimensão (Calendário, Fornecedores, Produtos) devidamente relacionadas para garantir performance nas consultas[cite: 4].
* **Layout do Relatório (`Report/Layout`)**: Telas planejadas com foco na experiência do usuário (UX), priorizando a leitura de dados da esquerda para a direita e de cima para baixo[cite: 4].
* **Identidade Visual (`CY26SU05.json`)**: Tema customizado aplicado diretamente aos recursos visuais para manter a consistência de cores, fontes e espaçamentos do relatório[cite: 4].
* **Metadados e Segurança (`Metadata` / `SecurityBindings`)**: Configurações internas que garantem a integridade do arquivo, controle de acessos e a correta vinculação dos esquemas de dados[cite: 4].

---

##  Principais Indicadores (KPIs) Analisados

O dashboard foi projetado para responder a perguntas de negócio cruciais através dos seguintes indicadores:

1. **Volume Total de Compras ($):** Valor bruto investido em aquisições no período selecionado.
2. **Ticket Médio por Pedido:** Média de gasto por transação efetuada.
3. **Quantidade de Pedidos/Itens:** Volume físico movimentado pelo setor de suprimentos.
4. **Lead Time de Entrega:** Período entre a emissão do pedido de compra e o recebimento da mercadoria.
5. **Concentração de Fornecedores:** Percentual de compras alocado nos principais parceiros (Curva ABC).

---

##  Páginas do Dashboard

O relatório está dividido em visões complementares para facilitar a navegação:

### 1. Visão Geral (Overview)
* Resumo dos principais KPIs de compras do período.
* Gráfico de linha demonstrando a evolução temporal dos gastos (sazonalidade).
* Filtros dinâmicos por período (ano, mês, trimestre), categoria de produto e filial.

### 2. Análise de Fornecedores
* Ranking dos fornecedores mais acionados e maior volume financeiro recebido.
* Matriz de dispersão cruzando o volume de compras com o nível de atraso nas entregas.
* Filtro detalhado por região geográfica do fornecedor.

### 3. Detalhes Operacionais
* Tabela analítica listando todas as notas fiscais, itens comprados, preços unitários e status do pedido.
* Ideal para auditorias e consultas rápidas do time operacional.

---

##  Tecnologias Utilizadas

* **Power BI / Microsoft Fabric:** Para modelagem, cálculo de métricas e visualização de dados[cite: 4].
* **Linguagem DAX (Data Analysis Expressions):** Utilizada na criação de medidas dinâmicas de inteligência temporal (ex: comparação de compras ano contra ano - *YoY*).
* **Power Query (M Language):** Utilizado na etapa de extração, transformação e limpeza dos dados (ETL).

---

##  Como Visualizar o Dashboard

1. Certifique-se de ter o **Power BI Desktop** instalado em sua máquina.
2. Baixe o arquivo `.pbix` ou `.pbit` disponível neste repositório.
3. Ao abrir o arquivo, o modelo processará o layout estruturado (`Report/Layout`) e carregará os metadados associados[cite: 4].
4. Utilize o painel de filtros na lateral direita de cada página para navegar entre os diferentes períodos de tempo e categorias de análise.

---

##  Notas de Versão

* **Versão Atual:** 1.0.0
* **Tema Base:** CY26SU05[cite: 4]
* **Status do Projeto:** Concluído / Fictício
