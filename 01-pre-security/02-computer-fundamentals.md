# Module 2: Computer Fundamentals

**Trilha:** Pre Security
**Status:** ✅ Concluído
**Período:** 12/10/2026 a 02/11/2026

[← Voltar ao README](../../README.md)

---

## Salas

| Sala | Data |
|---|---|
| Inside a Computer System | 12/10/2026 |
| Computer Types | 02/11/2026 |
| Client-Server Basics | 02/11/2026 |
| Virtualisation Basics | 02/11/2026 |
| Cloud Computing Fundamentals | 02/11/2026 |

---

## Inside a Computer System ✅

**O que aprendi**
- Componentes do computador: CPU, RAM, armazenamento (HD/SSD), PSU e placa-mãe
- Diferença entre firmware, UEFI e BIOS
- Sequência de boot: power button → firmware → POST → boot device → bootloader → OS

**Dificuldade:** associar os nomes dos componentes em inglês (CPU, GPU, PSU, motherboard, storage). Preciso revisar esse vocabulário técnico.

![Inside a Computer System](../../images/inside-a-computer-system-complete.jpg)

---

## Computer Types ✅

**O que aprendi**
- Diferenças práticas entre Laptop, Desktop, Workstation e Server, e o propósito de design de cada um
- *Trade-off* no hardware: mobilidade custa energia e capacidade de resfriamento, enquanto servidores priorizam redundância e desempenho contínuo
- **IoT** (conectado à rede para enviar dados e receber comandos, como câmeras e smart TVs) versus **Embedded Computers** (embutido em máquinas para executar uma função local, sem necessariamente ter conexão com a internet, como o sensor de uma porta automática)

**Dificuldade:** no início achei que tudo se resumia a IoT. A diferença está na conectividade com a rede.

**Lição-chave:** não existe o "melhor computador", existe a ferramenta certa para cada trabalho. O design de cada máquina reflete sua necessidade de mobilidade, poder de processamento ou confiabilidade.

![Computer Types](../../images/computer-types-complete.jpg)

---

## Client-Server Basics ✅

**O que aprendi**
- Modelo **Client-Server**: a comunicação na web funciona como um delivery (o cliente faz o pedido, o servidor responde)
- **Portas**: identificam o serviço específico rodando no servidor
- **DNS**: traduz nomes de domínio para endereços IP, como um GPS
- **Protocolo**: as regras e a linguagem acordadas entre cliente e servidor para que requisição e resposta funcionem
- **HTTP (GET)** na prática: usei as DevTools do navegador, dentro da máquina virtual, para inspecionar requisições, cabeçalhos (headers) e o status `200 OK`

**Observação:** primeira vez usando a máquina virtual integrada do TryHackMe.

**Lição-chave:** toda comunicação na web é baseada em requisições e respostas padronizadas. Entender como o navegador monta um request e como o servidor responde é a base para analisar qualquer tráfego de rede no futuro.

![Client-Server Basics](../../images/client-server-basics-complete.jpg)

---

## Virtualisation Basics ✅

**O que aprendi**
- O problema do "um servidor = uma aplicação" e como a virtualização resolve isso, otimizando o uso do hardware físico (menos desperdício de CPU, memória e custo)
- **Hypervisor**: software que gerencia e aloca recursos. **Type 1** (bare-metal) é usado em servidores e produção, e **Type 2** (hospedado em um SO, como o VirtualBox) em estudos e testes
- **VMs vs Containers**: VMs simulam um computador inteiro, com seu próprio SO. Containers compartilham o kernel do SO hospedeiro, por isso são mais leves e rápidos
- Prática no Virtualization Manager (ambiente simulado): reiniciei VMs com erro, criei uma nova máquina e analisei o consumo de hardware dos servidores físicos

**Dificuldade:** entender containers na teoria, porque o texto em inglês estava denso. A analogia dos "quartos dentro do apartamento" ajudou a fixar a ideia.

**Lição-chave:** a virtualização oferece máxima separação e flexibilidade (VMs completas), enquanto os containers oferecem leveza e agilidade para implantar aplicações. Saber escolher entre eles otimiza a infraestrutura.

![Virtualisation Basics](../../images/virtualisation-basics-complete.jpg)

---

## Cloud Computing Fundamentals ✅

**O que aprendi**
- Evolução da infraestrutura: servidores físicos → virtualização → nuvem, e como a nuvem resolveu problemas de custo e de limitação física
- Benefícios do modelo: escalabilidade, uso sob demanda (*on-demand*), pagamento pelo uso (*pay-as-you-go*) e alta disponibilidade
- Modelos de implantação (**Public, Private e Hybrid**) e modelos de serviço (**IaaS, PaaS e SaaS**), com a analogia do aluguel
- Prática em um console simulado estilo AWS: criei e gerenciei instâncias EC2, escolhi tipos de instância (t3.micro, m5.large) e acompanhei os custos

**Observação:** já tinha uma base de Cloud pelos cursos do Google Cloud que concluí.

**Lição-chave:** a nuvem não é sobre *onde* o servidor está, mas sobre *como* os recursos são consumidos. A abstração do hardware físico (via virtualização e containers) permite escalar aplicações em minutos e pagar apenas pelo que se usa.

![Cloud Computing Fundamentals](../../images/cloud-computing-fundamentals-complete.jpeg)

---

## 📝 Resumo do módulo

Este módulo consolidou como a infraestrutura de TI funciona, do nível mais baixo ao mais alto:

1. **Hardware:** como a máquina funciona por dentro, e como o design de cada computador é um *trade-off* focado no seu propósito
2. **Comunicação:** como as máquinas conversam via Client-Server, com protocolos (HTTP), portas e DNS
3. **Virtualização:** em vez de "um servidor físico por aplicação", *Hypervisors* criam VMs e *Containers* rodam software de forma isolada e eficiente
4. **Cloud:** a virtualização evoluiu para a nuvem, com os modelos IaaS, PaaS e SaaS e a possibilidade de escalar pagando só pelo uso

**Conclusão:** ir de "peças de computador" até "como a nuvem funciona" em um único módulo mostrou que a cibersegurança, especialmente o Blue Team, exige entender a fundação da infraestrutura antes de tentar defendê-la.
