<div align="center">

# Guilherme Dambroski

**Analista de Dados Sênior | Analytics Engineer**

[![Portfólio](https://img.shields.io/badge/Portfólio-guilherme--dambroski.web.app-0f172a?style=flat-square&logo=google-chrome&logoColor=38bdf8)](https://guilherme-dambroski.web.app/pt-br/data)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-guilherme--dambroski-0f172a?style=flat-square&logo=linkedin&logoColor=0077b5)](https://www.linkedin.com/in/guilherme-dambroski/)
[![Experiência](https://img.shields.io/badge/Carreira-5%20anos%20de%20experiência-0f172a?style=flat-square&logo=codewars&logoColor=34d399)](https://guilherme-dambroski.web.app/pt-br/data)
[![Modalidade](https://img.shields.io/badge/Regime-100%25%20Remoto-0f172a?style=flat-square&logo=linux&logoColor=f43f5e)](https://guilherme-dambroski.web.app/pt-br/data)

</div>

---

### Visão Geral

Com **5 anos de experiência**, atuo conectando engenharia analítica, modelagem dimensional e inteligência de negócios à tomada de decisão executiva. Meu foco prático está em desenhar pipelines determinísticos, eliminar gargalos de processamento em grandes volumes de dados e entregar camadas analíticas confiáveis para Produto, Customer Success, Operações e Diretoria.

Construo arquiteturas no modelo Medallion (Bronze, Silver e Gold) priorizando simplicidade operacional: processamento local e ágil com DuckDB e dbt quando o objetivo é velocidade e validação rápida de regras, e escalabilidade em nuvem (AWS S3, Glue e Athena) quando a demanda envolve grandes volumes e governança centralizada.

---

### Stack Técnica

| Domínio | Ferramentas & Tecnologias |
| :--- | :--- |
| **Engenharia Analítica & Modelagem** | dbt Core, DuckDB, Apache Airflow, Modelagem Dimensional (Star Schema), Arquitetura Medallion |
| **SQL & Bancos de Dados** | SQL Avançado (CTEs complexas, Window Functions, Query Tuning), PostgreSQL, SQL Server |
| **Business Intelligence & Dashboards** | Amazon QuickSight (QuickSight Embedded, RLS, SPICE), Power BI, Tableau Cloud, Excel Avançado |
| **Cloud & Armazenamento** | AWS (S3, Glue, Athena), GCP / BigQuery (consultas operacionais e validações analíticas diárias) |
| **Ambiente, Automação & Infra** | Python (automação e pipelines), Bash/Shell, Docker, Linux (CachyOS LTO, ZimaOS Homelab) |

---

### Casos Reais & Engenharia em Destaque

#### 1. [Quality Gate B3 com DuckDB e dbt Core (Código Aberto)](https://github.com/guilherme-dambroski/neoway)
- **Cenário:** Processamento e consolidação de cotações de pregão da B3 com inconsistências cadastrais de fontes públicas.
- **Decisão:** Estruturação de pipeline analítico em dbt Core + DuckDB conteinerizado via Docker e orquestrado por Airflow. Implementação de 17 testes de integridade (`dbt test`), identificando e tratando duplicações de CNPJs zerados (`cnpj <> '00000000000000'`) que inflavam as visualizações analíticas em mais de 80 mil registros.
- **Resultado:** 100% dos testes críticos aprovados determinísticamente antes da publicação para consumo em BI, com zero overhead de infraestrutura cloud paga para desenvolvimento local.

#### 2. Otimização de Performance SQL (3 minutos para 10 segundos)
- **Cenário:** Rotinas diárias de análise de churn e retenção de receita na Locaweb/Wake com consultas complexas demorando mais de 3 minutos por execução.
- **Decisão:** Refatoração estrutural de queries SQL, eliminação de subqueries redundantes, reescrita de agregações em Window Functions e otimização de joins na camada de consumo.
- **Resultado:** Redução de 98% no tempo de processamento das análises (de 3 minutos para 10 segundos) e alívio direto de 30% no backlog de solicitações analíticas do time de Customer Success.

#### 3. Arquitetura Medallion e Ingestão Cloud (AWS S3, Glue e Athena)
- **Cenário:** Cargas transacionais distribuídas em SQL Server sem camada analítica unificada, gerando concorrência em ambiente de produção e lentidão em relatórios.
- **Decisão:** Implementação de pipeline Medallion, extraindo dados operacionais para camada Bronze no AWS S3, enriquecimento e tipagem na Silver via catalogação no AWS Glue, e disponibilização de marts analíticos na Gold consultáveis via AWS Athena.
- **Resultado:** Desacoplamento total dos relatórios operacionais do banco transacional, viabilizando consultas analíticas sob demanda sem impacto na aplicação cliente.

#### 4. BI Corporativo em Escala com Segurança RLS (50+ Dashboards)
- **Cenário:** Necessidade de distribuir visões analíticas de vendas, estoque e churn para múltiplos clientes corporativos e lideranças internas com isolamento estrito de dados.
- **Decisão:** Desenvolvimento de mais de 50 dashboards corporativos em Amazon QuickSight e Power BI, implementando QuickSight Embedded com Row-Level Security (RLS) baseada no perfil e filial do usuário autenticado.
- **Resultado:** Visão unificada com governança ponta a ponta, garantindo que cada gestor visualize exclusivamente seus indicadores com atualização automática de métricas.

---

### Contato & Portfólio

- **Portfólio Web:** [guilherme-dambroski.web.app/pt-br/data](https://guilherme-dambroski.web.app/pt-br/data)
- **LinkedIn:** [linkedin.com/in/guilherme-dambroski](https://www.linkedin.com/in/guilherme-dambroski)
- **E-mail:** [guilherme.dambroski7@gmail.com](mailto:guilherme.dambroski7@gmail.com)
