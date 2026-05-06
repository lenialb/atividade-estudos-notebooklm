# ☁️ Cloud Cost Optimization and FinOps Principles Guide

## 🎯 Contexto e Objetivos
Este repositório foi criado como parte do desafio da DIO para explorar o uso da Inteligência Artificial e do **NotebookLM** como ferramenta de aprendizagem ativa.  
O tema escolhido foi **Cloud Cost Optimization e Princípios de FinOps**, com foco na plataforma AWS.  

**Objetivo principal:**  
Preparar-se para a certificação **FinOps Certified Practitioner (FOCP)**, consolidando os conceitos fundamentais de FinOps e aplicando-os às ferramentas nativas da AWS para otimização de custos.

---

## 📚 Curadoria de Fontes
Foram selecionadas **20 fontes** abertas em texto e PDF, que detalham estratégias e ferramentas para o gerenciamento financeiro na nuvem.  
O caderno temático foi organizado no NotebookLM e pode ser acessado aqui:  
👉 [NotebookLM - Cloud Cost Optimization and FinOps Principles Guide](https://notebooklm.google.com/notebook/64b3b418-4652-4546-b88a-4b7a1346a13b)

Principais tópicos abordados nas fontes:
- Diferenças entre **Savings Plans** e **Reserved Instances**.  
- Uso de ferramentas como **AWS Cost Explorer**, **Trusted Advisor** e **Budgets**.  
- Importância da mudança cultural e colaboração entre equipes de tecnologia e finanças.  
- Diretrizes do **AWS Well-Architected Framework** para governança financeira contínua.  

---

## 🧩 Engenharia de Prompts e "Cicatrizes"
Durante os estudos, foram elaborados prompts estratégicos para extrair informações relevantes:

- **Prompt 1:** "Quais são as principais diferenças entre AWS Savings Plans e Reserved Instances?"  
- **Prompt 2:** "Como as ferramentas AWS Cost Explorer e Budgets auxiliam na otimização de custos?"  
- **Prompt 3:** "O que é FinOps e quais os benefícios
- **Prompt 4:** "Guia de Estudos Estruturado: FinOps Certified Practitioner (FOCP) com Foco em AWS"

# ☁️ Guia de Estudos Estruturado: FinOps Certified Practitioner (FOCP) com Foco em AWS

Este guia foi desenvolvido para fornecer um roteiro técnico e estratégico para profissionais que buscam a certificação **FinOps Certified Practitioner (FOCP)**.  
Como Arquiteto de Soluções AWS e Especialista em FinOps, o material integra o **FinOps Framework** da FinOps Foundation com as melhores práticas (BPs) do pilar de **Otimização de Custos** do AWS Well-Architected Framework.

---

## 1. Introdução ao FinOps e à Certificação

### 1.1 Definição e Mudança Cultural
- **FinOps** é uma disciplina em evolução que une tecnologia, finanças e negócios.  
- Objetivo: promover responsabilidade financeira e maximizar o valor de negócio da nuvem.  
- **Triângulo de Ferro (Iron Triangle):** equilíbrio entre Velocidade, Custo e Qualidade.  
- **FinOps e Sustentabilidade:** eficiência de custos reduz desperdício e pegada de carbono.

### 1.2 O Exame FOCP
- **Formato:** 50 questões de múltipla escolha.  
- **Duração:** 60 minutos.  
- **Pontuação mínima:** 75% (38 questões).  
- **Validade:** 24 meses.  

---

## 2. Domínio 1: Desafios da Nuvem e o Modelo de Consumo

### 2.1 Variabilidade vs. Previsibilidade
- TI tradicional: custos fixos (CapEx).  
- Nuvem: consumo variável (OpEx).  
- **Exemplo:** desligar ambientes de desenvolvimento fora do horário comercial gera economia de ~76%.

### 2.2 Desafios de Gestão
- Descentralização dos gastos.  
- Recursos ociosos (zombies).  
- Complexidade de faturamento.  
- Forecasting impreciso.

### 2.3 AWS Well-Architected Framework (Princípios de Custo)
- Adotar modelo de consumo.  
- Evitar gastos em tarefas genéricas.  
- Medir eficiência com **Unit Economics**.  

---

## 3. Domínio 2: Princípios do FinOps e Governança na AWS

### 3.1 Princípios Fundamentais
- Colaboração entre equipes.  
- Propriedade individual dos custos.  
- Relatórios em tempo real.  

### 3.2 Governança e Políticas (COST02-BP01)
- **Restrição Geográfica:** priorizar regiões específicas.  
- **Agendamento de Instâncias:** EC2/RDS entre 06:00 e 20:00.  
- **Inatividade:** encerrar instâncias após períodos definidos.  
- **Higiene de Ambiente:** regras diferentes para produção e não-produção.  

### 3.3 Metas e KPIs (COST02-BP02)
| Categoria     | KPI                        | Descrição |
|---------------|-----------------------------|-----------|
| Computação    | Cobertura de uso do EC2     | % coberta por SP/RI |
| Computação    | Última geração de instância | % usando Graviton ou gerações recentes |
| Computação    | Custo de vCPU              | Média de custo por unidade |
| Armazenamento | Utilização de armazenamento | Razão entre Glacier/Deep Archive e total |
| Banco de Dados| Cobertura de RDS            | % coberta por RIs |
| Tags          | Recursos não marcados       | Valor total sem tags no Cost Explorer |

---

## 4. Domínio 3: Equipes e Colaboração Interdisciplinar

### 4.1 Centro de Excelência da Nuvem (CCoE / FinOps Team)
- Modelos: Centralizado, Descentralizado ou Híbrido.  
- Patrocínio executivo é indispensável.  

### 4.2 Parceria Finanças e Tecnologia (COST01-BP02)
- Modelo tradicional substituído por parceria estratégica.  
- TI como operadora e proprietária do gasto.  
- Finanças como consultora de investimentos.  

---

## 5. Domínio 4: Capacidades e Ferramentas AWS de Relatórios

### 5.1 Visibilidade e Alocação
- **AWS Organizations:** faturamento consolidado.  
- **Tagging:** base da alocação de custos.  

### 5.2 Ferramentas de Monitoramento
- **AWS Cost Explorer:** tendências e previsões.  
- **AWS CUR:** dados granulares.  
- **AWS Cost Anomaly Detection:** alertas via ML.  
- **AWS Trusted Advisor:** recomendações de custo.  
- **AWS CloudTrail:** auditoria de custos.  
- **Amazon S3 Analytics:** padrões de acesso e transição de classes.  

---

## 6. Domínio 5: Ciclo de Vida FinOps (Inform, Optimize, Operate)

### 6.1 Fase Inform
- Visibilidade e alocação correta.  
- Forecasting com ML + business drivers.  

### 6.2 Fase Optimize
- Redução de custo unitário.  
- Comparativo de modelos de compromisso:

| Modelo                     | Flexibilidade | Desconto (1 ano) | Desconto (3 anos) | Marketplace |
|-----------------------------|---------------|------------------|-------------------|-------------|
| Compute Savings Plans       | Máxima        | 26% - 49%        | 42% - 66%         | Não         |
| EC2 Instance Savings Plans  | Média         | 28% - 52%        | 44% - 72%         | Não         |
| Standard RIs                | Baixa         | Até 41%          | Até 72% - 75%     | Sim         |
| Convertible RIs             | Média         | 23% - 41%        | 41% - 54%         | Não         |

**Estratégia:** combinar SP para cargas variáveis e RIs para workloads estáveis.  

---

## 7. Domínio 6: Terminologia e Conceitos de Preço

### 7.1 Glossário Essencial
- **FOCUS:** padrão open-source para dados de faturamento.  
- **Unit Economics:** custo por métrica de negócio.  
- **Showback vs. Chargeback:** conscientização vs. recuperação de custos.  

### 7.2 Reserva de Capacidade
- **Não reservam:** Savings Plans e Regional RIs.  
- **Reservam:** apenas Zonal RIs.  

---

## 8. Preparação Final e Recursos Recomendados

### 8.1 Dicas para o Sucesso
- FOCP foca em Framework e cultura.  
- Revise whitepapers da AWS.  
- Pratique leitura de faturas e uso das ferramentas.  

### 8.2 Recursos de Estudo
- **FinOps Foundation:** [finops.org](https://finops.org)  
- **Cursos Gratuitos:** Introduction to FinOps, Introduction to FOCUS.  
- **Livro:** *Cloud FinOps* (O'Reilly).  
- **Laboratórios:** Well-Architected Labs (Cost Optimization).  
- **Comunidade:** FinOps Foundation YouTube, grupos locais.  

---

## ✨ Autor
Projeto desenvolvido por **Lenilson** como parte do desafio da DIO.
