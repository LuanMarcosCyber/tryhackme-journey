# Module 3: Operating Systems Basics

**Trilha:** Pre Security
**Status:** ⏳ Em andamento
**Início:** 03/11/2026

[← Voltar ao README](../README.md)

---

## Salas

| Sala | Data |
|---|---|
| Operating Systems Introduction | 03/11/2026 |
| Windows Basics | 04/11/2026 |

---

## Operating Systems Introduction ✅

**O que aprendi**
- O **Sistema Operacional (OS)** é o "gerente invisível" que faz a ponte entre hardware, aplicações e usuário
- Separação de privilégios: **Kernel Space** (acesso irrestrito ao hardware, como a torre de controle de um aeroporto) e **User Space** (onde os aplicativos rodam de forma isolada e segura)
- Principais responsabilidades do OS: gerenciamento de processos (multitarefa), memória (RAM e virtual), arquivos, usuários e dispositivos (drivers)
- Panorama dos sistemas operacionais no mundo real (Desktop, Server, Mobile, Embedded, Virtual/Cloud) e a diferença entre **GUI** (interface gráfica) e **CLI** (linha de comando)
- Prática em um ambiente Linux (Ubuntu Mate) na máquina virtual: usei a GUI para verificar informações do sistema (versão, hardware, memória) e navegar por diretórios

**Dificuldade:** associar as responsabilidades do OS a exemplos práticos do dia a dia e se orientar na estrutura de pastas do Linux.

**Lição-chave:** sem o OS, o hardware seria apenas um monte de metal inútil. A separação entre Kernel e User Space garante a estabilidade do sistema (se um app travar, não derruba a máquina inteira) e é a base da segurança da informação.

![Operating Systems Introduction](../images/operating-systems-introduction-complete.jpg)

---

## Windows Basics ✅

**O que aprendi**
- Interface do Windows Server 2019 e estrutura de contas de usuário (Guest, Standard e Administrator), com a importância da autenticação
- **File Explorer**: gerenciar arquivos, entender caminhos (*paths*) e instalar/desinstalar aplicações
- **Gerenciador de Tarefas (Task Manager)**: analisar processos em segundo plano, uso de CPU/RAM e contas de usuário logadas
- **Windows Security**: fiz uma varredura personalizada (*custom scan*) em uma pasta específica e a ferramenta identificou e isolou o arquivo de teste `Virus:DOS/EICAR_Test_File`, uma ameaça simulada
- **Windows Defender Firewall**: regras de entrada e saída, e como os perfis de rede (Domain, Private, Public) protegem o sistema

**Descoberta:** não sabia que o Windows Security fazia varreduras direcionadas, e nunca tinha ido além da aba de aplicativos abertos no Gerenciador de Tarefas.

**Lição-chave:** o Windows tem ferramentas nativas de defesa e monitoramento poderosas (Defender e Task Manager), que são o primeiro passo para qualquer análise de Blue Team. Saber onde olhar e como configurar essas ferramentas é essencial para identificar anomalias.

![Windows Basics](../images/windows-basics-complete.jpg)

---

## Linux CLI Basics ✅

**O que aprendi**
- **Terminal (CLI) na cibersegurança:** oferece mais controle, velocidade e acesso a ferramentas que não têm interface gráfica
- **Navegação no sistema de arquivos:** `pwd` (onde estou), `ls` (listar arquivos; `ls -a` mostra os ocultos e `ls -l` os detalhes) e `cd` (mudar de diretório)
- **Busca e leitura de arquivos:** `find ~ -name "arquivo"` procura um arquivo pelo nome a partir da pasta pessoal (`~`), e `cat` mostra o conteúdo
- **Informações do sistema:** `whoami` (usuário atual), `uname -a` (kernel e máquina) e `df -h` (uso de disco em formato legível)

**Dificuldade:** lembrar a sintaxe exata do `find` no desafio final. Esqueci que o comando precisa do diretório de busca e da flag `-name` (`find ~ -name "arquivo"`), e só consegui resolver depois de revisar a estrutura.

**Lição-chave:** o terminal exige precisão. Esquecer o diretório de busca ou uma flag faz o comando falhar. A repetição constrói a memória muscular para comandos como `find`, `ls` e `cat`, que serão a base das investigações em Linux daqui pra frente.

![Linux CLI Basics](../images/linux-cli-basics-complete.jpg)

---
