# Resumo-do-lab
Este repositório contém o resumo das lições aprendidas durante o desenvolvimento do lab na DIO.

# 🌐 Introdução a Computação em Nuvem

## 👨‍💻 Heliton de Pontes Mendes

Como um **especialista em desenvolvimento de sistemas**, atuo com foco em soluções escaláveis, seguras e orientadas a resultados.  
Minha experiência abrange desde o **planejamento de arquiteturas de software** até a **implantação de ambientes em nuvem**, sempre utilizando as melhores práticas de engenharia de software e DevOps.

Sou também **especialista em engenharia de software e DevOps**, com expertise em:
- Automação de pipelines CI/CD;
- Monitoramento e observabilidade de aplicações;
- Integração contínua entre desenvolvimento e operações;
- Adoção de metodologias ágeis e cultura DevOps.

---

## ☁️ Introdução aos Serviços em Nuvem — Microsoft Azure

A plataforma **Azure** oferece um vasto conjunto de serviços para suportar aplicações modernas, integradas e altamente disponíveis.  
A seguir, apresento uma visão organizada dos principais grupos de serviços:

### 1. **Serviços de Computação**
- **Azure Virtual Machines (VMs)** – Instâncias virtuais para hospedagem de sistemas e aplicações.
- **Azure App Service** – Hospedagem gerenciada para aplicações Web, APIs e mobile.
- **Azure Functions** – Execução de código sob demanda com arquitetura serverless.

### 2. **Serviços de Armazenamento**
- **Blob Storage** – Armazenamento de objetos não estruturados, ideal para imagens, vídeos e backups.
- **File Storage** – Armazenamento de arquivos com acesso via SMB.
- **Queue Storage** – Mensageria simples para comunicação entre componentes distribuídos.

### 3. **Serviços de Banco de Dados**
- **Azure SQL Database** – Banco de dados relacional totalmente gerenciado.
- **Cosmos DB** – Banco de dados NoSQL globalmente distribuído.
- **Azure Database for PostgreSQL/MySQL** – Serviços gerenciados para bancos open-source.

### 4. **Rede e Segurança**
- **Virtual Network (VNet)** – Criação de redes virtuais privadas e seguras.
- **Azure Firewall** – Proteção e controle de tráfego de rede.
- **Azure Active Directory (AAD)** – Gerenciamento de identidades e autenticação.

### 5. **DevOps e Integração Contínua**
- **Azure DevOps Services** – Pipelines, controle de versão e gestão de projetos.
- **GitHub Actions (integração com Azure)** – Automação de builds, testes e deploys.
- **Azure Monitor e Application Insights** – Monitoramento e métricas de desempenho.

# ☁️ Tipos de Serviços de Nuvem — Microsoft Azure

A computação em nuvem é estruturada em diferentes **modelos de serviço**, que definem o nível de controle, responsabilidade e flexibilidade entre o provedor e o cliente.  
Os três principais modelos são: **IaaS**, **PaaS** e **SaaS** — além de extensões modernas como **FaaS** e **CaaS**.

---

## 🧱 Modelos Clássicos de Serviços em Nuvem

| 🏷️ Tipo de Serviço | 🧩 Nome Completo | ⚙️ Responsabilidade do Usuário | ☁️ Responsabilidade do Provedor | 💡 Exemplos no Azure | 🚀 Casos de Uso |
|--------------------|-----------------|--------------------------------|----------------------------------|----------------------|----------------|
| **IaaS** | Infrastructure as a Service | Sistema operacional, middleware, runtime, aplicações e dados | Rede, armazenamento, servidores e virtualização | Azure Virtual Machines, Azure Storage, Virtual Network | Hospedagem de servidores, ambientes de teste, migração de infraestrutura física. |
| **PaaS** | Platform as a Service | Aplicações e dados | Rede, armazenamento, servidores, SO, middleware, runtime | Azure App Service, Azure SQL Database, Azure Functions | Desenvolvimento e hospedagem de aplicações web, APIs e microserviços. |
| **SaaS** | Software as a Service | Uso do software (sem necessidade de gerenciar infraestrutura ou plataforma) | Todo o ambiente e aplicação | Microsoft 365, Dynamics 365, Power BI | Aplicações prontas para uso, produtividade, CRM, BI. |

---

## ⚙️ Modelos Modernos e Complementares

| 🏷️ Tipo de Serviço | 🧩 Nome Completo | 💡 Conceito | 💻 Exemplos no Azure | 🚀 Casos de Uso |
|--------------------|-----------------|-------------|----------------------|----------------|
| **FaaS** | Function as a Service | Execução de código sob demanda (serverless), pagando apenas pelo uso | Azure Functions | Automação de eventos, backend sem servidor, integrações rápidas. |
| **CaaS** | Container as a Service | Gerenciamento de contêineres e orquestração de clusters | Azure Kubernetes Service (AKS) | Aplicações em microserviços, pipelines CI/CD, escalabilidade dinâmica. |
| **DBaaS** | Database as a Service | Banco de dados totalmente gerenciado | Azure SQL Database, Cosmos DB | Gerenciamento de dados com alta disponibilidade e backup automático. |
| **BaaS** | Backend as a Service | Backend pronto com autenticação, APIs e armazena

---
## 🚀 Benefícios da Adoção do Azure
- Alta disponibilidade e escalabilidade global;  
- Segurança de nível corporativo e conformidade;  
- Redução de custos operacionais com recursos sob demanda;  
- Integração facilitada com ferramentas DevOps e serviços Microsoft;  
- Suporte completo a múltiplas linguagens e frameworks.

# ☁️ SLA dos Principais Serviços da Plataforma Microsoft Azure

| 🧩 Serviço | 🔒 Nível de Disponibilidade (SLA) | 📘 Detalhes / Condições |
|------------|----------------------------------|--------------------------|
| **Máquinas Virtuais (VMs)** | - 99,99% com 2+ instâncias em **Availability Zones**<br>- 99,95% com 2+ instâncias em **Availability Set**<br>- 99,9% (Single Instance com **Premium SSD/Ultra Disk**)<br>- 99,5% (Single Instance com **Standard SSD**)<br>- 95% (Single Instance com **HDD**) | SLA de conectividade garantida a pelo menos uma instância virtual em execução. |
| **Azure SQL Database** | **99,995%** (camada *Business Critical* ou com redundância de zona) | Garantia de alta disponibilidade com RPO de 5s e RTO de 30s em bancos geo-replicados. |
| **Azure SQL Managed Instance** | **99,99%** | Disponibilidade garantida para instâncias configuradas corretamente em ambientes General Purpose e Business Critical. |
| **Azure App Service / Web Apps** | - **99,99%** com *Availability Zones*<br>- **99,95%** sem zonas | Hospedagem gerenciada de aplicações web e APIs com failover automático. |
| **Azure Kubernetes Service (AKS)** | **99,95%** (clusters com 2+ nós e zonas de disponibilidade) | Garantia de disponibilidade do *API Server* e do *control plane*. |
| **Azure Storage (Blob, Files, Queue, Table)** | **99,99%** (armazenamento local redundante - LRS)<br>**99,999999999%** (durabilidade dos dados) | Alta durabilidade com replicação automática e redundância geográfica opcional. |
| **Azure Load Balancer** | **99,99%** | SLA de disponibilidade para balanceamento interno e externo de tráfego. |
| **Azure VPN Gateway** | **99,95%** | SLA de conectividade entre redes virtuais e locais. |
| **Azure Active Directory (AAD)** | **99,99%** | SLA para autenticação, gerenciamento de identidades e single sign-on. |
| **Azure DNS** | **100%** | SLA de disponibilidade total para resolução e gerenciamento de DNS hospedado no Azure. |
| **Azure DevOps Services** | **99,9%** | Garantia de disponibilidade dos serviços de pipelines, repositórios e boards. |

---

> 🧠 **Observação:** Os valores de SLA podem variar conforme a região, configuração do serviço e tipo de contrato.  
> Sempre consulte a documentação oficial atualizada em:  
> [https://azure.microsoft.com/support/legal/sla](https://azure.microsoft.com/support/legal/sla)



---

# ☁️ Exemplos Práticos de Aplicações em Nuvem — Microsoft Azure

A computação em nuvem permite que empresas e desenvolvedores criem soluções escaláveis, seguras e disponíveis globalmente.  
A seguir, apresentamos **5 exemplos reais de aplicações na nuvem** e como elas utilizam os serviços do Microsoft Azure.

---

## 🧩 1. Aplicação Web Escalável
**Tipo de serviço:** Platform as a Service (PaaS)

**Serviços Azure utilizados:**
- Azure App Service  
- Azure SQL Database  
- Azure Application Insights  

**Descrição:**
Aplicação web corporativa hospedada no Azure App Service, com banco de dados relacional em Azure SQL.  
A solução pode escalar automaticamente durante picos de acesso.

**Benefícios:**
- Escalabilidade automática sob demanda;  
- Baixo custo operacional;  
- Monitoramento em tempo real.  

**Caso de uso:**  
Portal de vendas online que suporta milhares de acessos simultâneos em campanhas promocionais.

---

## ⚙️ 2. Infraestrutura Virtualizada para ERP
**Tipo de serviço:** Infrastructure as a Service (IaaS)

**Serviços Azure utilizados:**
- Azure Virtual Machines  
- Virtual Network  
- Azure Backup  

**Descrição:**
Hospedagem de um sistema ERP corporativo em VMs do Azure, com controle total sobre o sistema operacional e rede.

**Benefícios:**
- Alta disponibilidade (SLA de 99,99%);  
- Recuperação rápida em caso de falha;  
- Flexibilidade para customizações.  

**Caso de uso:**  
Ambiente de produção para sistema ERP TOTVS, SAP ou Oracle em nuvem híbrida.

---

## 🤖 3. Chatbot Inteligente com IA
**Tipo de serviço:** AI as a Service (AIaaS)

**Serviços Azure utilizados:**
- Azure Bot Service  
- Azure Cognitive Services (Language, Speech)  
- Azure OpenAI Service  

**Descrição:**
Chatbot inteligente para atendimento automatizado ao cliente, com reconhecimento de linguagem natural e voz.

**Benefícios:**
- Redução de custos operacionais;  
- Atendimento 24/7;  
- Integração com sites, WhatsApp e Teams.  

**Caso de uso:**  
Assistente virtual de suporte técnico para empresas de telecomunicações.

---

## 📦 4. Armazenamento e Backup Corporativo
**Tipo de serviço:** Storage as a Service (STaaS)

**Serviços Azure utilizados:**
- Azure Blob Storage  
- Azure Files  
- Azure Backup  

**Descrição:**
Sistema de backup e armazenamento de grandes volumes de arquivos e logs corporativos.

**Benefícios:**
- Alta durabilidade (11 noves de confiabilidade);  
- Acesso seguro via chave e token;  
- Integração com sistemas locais.  

**Caso de uso:**  
Backup automatizado de servidores físicos e dados de clientes em escritórios remotos.

---

## 📊 5. Análise de Dados e BI em Tempo Real
**Tipo de serviço:** Platform + Software as a Service (PaaS + SaaS)

**Serviços Azure utilizados:**
- Azure Synapse Analytics  
- Power BI  
- Azure Data Lake Storage  

**Descrição:**
Pipeline de dados em tempo real integrando fontes internas e externas para dashboards de inteligência de negócios.

**Benefícios:**
- Insights instantâneos sobre operações;  
- Conectividade com múltiplas fontes;  
- Dashboards interativos e acessíveis via navegador.  

**Caso de uso:**  
Análise de desempenho de vendas e comportamento de clientes em tempo real.

---
# ☁️ Tutorial: Como Criar uma Máquina Virtual no Microsoft Azure

> 📘 **Objetivo:**  
Aprender a criar, configurar e acessar uma Máquina Virtual (VM) no Microsoft Azure, passo a passo, utilizando o portal web.

---

## 🧩 1. Acessar o Portal do Azure

1. Acesse o portal oficial: [https://portal.azure.com](https://portal.azure.com)
2. Faça login com sua conta Microsoft (corporativa ou pessoal).
3. Após o login, você verá o **Dashboard do Azure**.

![Portal do Azure](https://learn.microsoft.com/en-us/azure/virtual-machines/media/quick-create-portal/portal-home.png)

---

## ⚙️ 2. Criar um Novo Recurso

1. No menu lateral esquerdo, clique em **“Criar um recurso”**.
2. Digite **“Máquina Virtual”** na barra de pesquisa e selecione a opção **Virtual Machine**.
3. Clique em **“Criar”** para iniciar a configuração.

![Criar Recurso](https://learn.microsoft.com/en-us/azure/virtual-machines/media/quick-create-portal/search-vm.png)

---

## 🧱 3. Configurar a Máquina Virtual

### 🗂️ Aba “Noções Básicas”
Preencha as informações iniciais:
- **Assinatura:** escolha a conta de faturamento.
- **Grupo de Recursos:** crie um novo ou selecione um existente.
- **Nome da VM:** defina um nome amigável, como `vm-treinamento`.
- **Região:** escolha a região mais próxima (ex: *Brazil South*).
- **Imagem:** selecione o sistema operacional (ex: *Windows Server 2022* ou *Ubuntu 22.04 LTS*).
- **Tamanho:** escolha o tipo de hardware (ex: *B1s*, *D2s_v3*).

![Configuração Básica](https://learn.microsoft.com/en-us/azure/virtual-machines/media/quick-create-portal/basics.png)

---

## 🔐 4. Definir Credenciais de Acesso

Escolha o método de autenticação:
- **Usuário e senha** (para Windows/Linux)
- **Chave pública SSH** (recomendado para Linux)

⚠️ **Dica:**  
Anote o nome de usuário e senha/chave SSH — você precisará delas para acessar a VM.

![Credenciais](https://learn.microsoft.com/en-us/azure/virtual-machines/media/quick-create-portal/ssh-key.png)

---

## 🌐 5. Configurar Rede e Segurança

Na aba **Rede**:
- Mantenha a **rede virtual padrão** ou crie uma nova.
- Habilite o **acesso à porta 22 (SSH)** para Linux ou **porta 3389 (RDP)** para Windows.

![Rede e Porta](https://learn.microsoft.com/en-us/azure/virtual-machines/media/quick-create-portal/network.png)

---

## 💾 6. Revisar e Criar

1. Clique em **“Revisar + Criar”**.
2. O Azure validará as configurações.
3. Clique em **“Criar”** para iniciar a implantação da VM.

O processo de criação leva alguns minutos.

![Revisar e Criar](https://learn.microsoft.com/en-us/azure/virtual-machines/media/quick-create-portal/review.png)

---

## 🖥️ 7. Conectar-se à Máquina Virtual

Após a implantação:
1. Vá até o recurso criado.
2. Clique em **“Conectar”**.
3. Escolha:
   - **RDP** (Windows)  
   - **SSH** (Linux)

Exemplo de conexão via SSH:
```bash
ssh azureuser@<ip-publico>




> 💡 *A computação em nuvem é o alicerce da transformação digital moderna, e o Azure se destaca por sua flexibilidade, segurança e integração com o ecossistema Microsoft.*


