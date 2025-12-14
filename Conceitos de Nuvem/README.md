# Conceitos de Nuvem

## Modelos de Nuvem

**O que é computação em nuvem?**
Computação em nuvem é a entrega de serviços de computação pela Internet, proporcionando inovação mais rápida, recursos flexíveis e economia de escala.

Principais categorias de recursos: **Computação, Rede, Armazenamento e Análise**.

## Tipos de Serviço de Nuvem

### 🧱 IaaS – Infrastructure as a Service (Infraestrutura como Serviço)

* Fornece recursos básicos de computação: **máquinas virtuais, redes, armazenamento**.
* O cliente gerencia: SO, aplicativos, dados.
* Exemplo: Azure Virtual Machines, Azure Storage.
* O serviço de nuvem mais flexível.
* Você configura e gerencia o hardware para seu aplicativo.

### 🧩 PaaS – Platform as a Service (Plataforma como Serviço)

* Fornece ambiente gerenciado para criar, testar e implantar aplicativos.
* O cliente gerencia apenas o código e dados.
* Exemplo: Azure App Service, Azure Functions, Azure SQL Database.
* Focado no desenvolvimento de aplicativos.
* O gerenciamento de plataforma é realizado pelo provedor de nuvem.

### 📦 SaaS – Software as a Service (Software como Serviço)

* Software pronto, acessado pela Internet.
* O provedor gerencia tudo.
* Exemplo: Microsoft 365, Dynamics 365.
* Modelo de preço pago conforme o uso.
* Os usuários pagam pelo software que utilizam em um modelo de assinatura.

## Modelo de Responsabilidade Compartilhada

| Responsabilidade | IaaS       | PaaS       | SaaS       |
| ---------------- | ---------- | ---------- | ---------- |
| Aplicativo       | ✔️ Cliente | ✔️ Cliente | ❌ Provedor |
| Dados            | ✔️ Cliente | ✔️ Cliente | ❌ Provedor |
| Runtime          | ✔️ Cliente | ❌ Provedor | ❌ Provedor |
| Middleware       | ✔️ Cliente | ❌ Provedor | ❌ Provedor |
| SO               | ✔️ Cliente | ❌ Provedor | ❌ Provedor |
| Virtualização    | ❌ Provedor | ❌ Provedor | ❌ Provedor |
| Servidores       | ❌ Provedor | ❌ Provedor | ❌ Provedor |
| Armazenamento    | ❌ Provedor | ❌ Provedor | ❌ Provedor |
| Rede             | ❌ Provedor | ❌ Provedor | ❌ Provedor |

## Modelos de implantação

### ☁️ Nuvem Pública

Pertencente a um provedor de serviços de nuvem.

* Nenhuma despesa de capital para escalar verticalmente.
* Aplicativos podem ser provisionados e desprovisionados rapidamente.
* Pagamento apenas pelo que usar (modelo pay-as-you-go).

### 🏢 Nuvem Privada

Criada e mantida pela própria organização no datacenter.

* Requer aquisição e manutenção de hardware.
* Controle total sobre segurança e recursos.
* Responsabilidade completa por atualizações e manutenção.

### 🔗 Nuvem Híbrida

Combinação da nuvem pública e privada.

* Oferece maior flexibilidade.
* Permite escolher onde cada aplicativo será executado.
* Controle sobre segurança, conformidade e requisitos legais.

## CapEx e OpEx

### 💰 Despesas de Capital (CapEx)

* Gastos iniciais com infraestrutura física (servidores, datacenter, hardware).
* O custo é pago antecipadamente e depreciado ao longo do tempo.
* Normalmente exige grande investimento inicial.

### 🔄 Despesas Operacionais (OpEx)

* Custos contínuos, pagos conforme o uso.
* Não há necessidade de investir em hardware próprio.
* Muito utilizado em computação em nuvem.

## Modelo baseado em consumo

Os provedores de serviços de nuvem utilizam um **modelo baseado em consumo**, onde:

* O usuário paga apenas pelos recursos que realmente utilizar.
* Não há custos fixos obrigatórios.
* Facilita a **previsão e otimização de custos**, pois é possível ajustar o consumo conforme a demanda.

## Benefícios da Nuvem

### 🔹 Alta disponibilidade

É o **tempo que o serviço fica no ar**.

➡️ A nuvem é feita para **não parar**, usando:

* Datacenters redundantes
* Zonas de disponibilidade
* SLAs (99,9%, 99,99% etc.)

📌 *Exemplo:*
Mesmo se um datacenter cair, outro continua atendendo.

---

### 🔹 Escalabilidade

É a capacidade de **aumentar ou diminuir recursos conforme a demanda**.

Existem **dois tipos**:

#### 🔼 Escalabilidade vertical

* Aumentar **poder da máquina**
* Mais CPU, mais memória, mais disco

📌 Exemplo:
Trocar uma VM pequena por uma VM maior.

#### 🔁 Escalabilidade horizontal

* Aumentar ou reduzir a **quantidade de recursos**
* Mais VMs, mais contêineres, mais instâncias

📌 Exemplo:
Passar de 2 VMs para 10 VMs durante um pico de acesso.

💡 **Vantagem importante:**
Você **não paga além do necessário**, porque pode reduzir depois.

---

### 🔹 Confiabilidade

É a capacidade do sistema de **continuar funcionando mesmo quando algo falha**.

➡️ A nuvem é confiável porque:

* Usa redundância
* Replica dados
* Possui recuperação automática

📌 *Exemplo:*
Se um servidor falhar, outro assume automaticamente.

---

### 🔹 Previsibilidade

É a capacidade de **prever comportamento e custos**.

➡️ A nuvem oferece:

* SLAs claros
* Monitoramento
* Controle de gastos
* Escalabilidade planejada

📌 *Exemplo:*
Você sabe quanto vai pagar e qual nível de disponibilidade esperar.

---

### 🔹 Segurança

A nuvem oferece **segurança em várias camadas**:

* Criptografia
* Controle de acesso
* Monitoramento contínuo
* Conformidade com normas (LGPD, ISO, etc.)

📌 Importante para a prova:
👉 **Segurança é responsabilidade compartilhada** entre cliente e provedor.

---

### 🔹 Governança

É a capacidade de **definir regras e controlar o uso dos recursos**.

➡️ Inclui:

* Políticas
* Controle de acesso (RBAC)
* Padrões organizacionais
* Conformidade

📌 *Exemplo:*
Impedir que alguém crie recursos fora do padrão da empresa.

---

### 🔹 Capacidade de gerenciamento

É a facilidade de **monitorar, configurar e administrar tudo**.

➡️ A nuvem oferece:

* Portais gráficos
* CLI
* Automação
* Monitoramento centralizado

📌 *Exemplo:*
Gerenciar centenas de recursos pelo Portal do Azure ou scripts.