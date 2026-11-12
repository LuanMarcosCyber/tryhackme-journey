# Module 4: Software Basics

**Status do Módulo:** ⌛ Em Andamento

**Período:** 10/11/2026 - a concluir 

[← Voltar ao README](../README.md)

---

## Salas

| Sala | Data |
|---|---|
| Data Representation | 12/10/2026 |
| Data Enconding | ⌛ A fazer  |
| Python: Simple Demo | ⌛ A fazer |
| JavaScript: Simple Demo | ⌛ A fazer |
| Database SQL Basics | ⌛ A fazer  |

---
## Data Representation ✅

**O que aprendi**
- **Representação de cores:** de um modelo simples de 8 cores (1 bit por cor primária RGB) até o padrão de 24 bits (*True Color*), com 8 bits por canal, que gera mais de 16 milhões de cores
- **Sistema binário (Base-2):** cada posição vale uma potência de 2, e é assim que se converte binário em decimal
- **Sistema hexadecimal (Base-16):** agrupa 4 bits em um único caractere (0 a F), o que facilita a leitura de sequências binárias longas
- **Conversões** entre decimal, binário e hexadecimal (e octal, de forma opcional), com apoio das ferramentas Color Decoder e Base Converter

**Exemplos**
- Binário para decimal: `1011` = 8 + 0 + 2 + 1 = **11**
- Decimal para binário e hexa: `255` = `11111111` = `FF` (o valor máximo de 8 bits)
- Cores em hexa: `#FF0000` = vermelho no máximo (R = FF) e verde e azul zerados (G = 00, B = 00)

**Dificuldade:** foi a sala mais difícil até agora. Demorei para entender a lógica das conversões, principalmente entre binário e decimal nos dois sentidos, porque exige um raciocínio matemático com o qual eu não estava acostumado. Preciso praticar mais para fixar.

**Lição-chave:** o computador trabalha com dois estados (ligado e desligado, 0 e 1), e tudo o que ele guarda (cores, letras, arquivos) é uma tradução disso. A conversão entre bases importa para a segurança porque o hexadecimal aparece o tempo todo em endereços, hashes e na análise de pacotes e de malware.

![Data Representation](../images/data-representation.png)

---
