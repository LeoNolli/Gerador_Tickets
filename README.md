<div align="center">

# Automação de Emissão de Ingressos para Turismo

Este repositório contém a lógica de um sistema de automação desenvolvido no n8n para a geração dinâmica de tickets virtuais. A solução integra APIs nativas do Google Workspace para criar um fluxo de trabalho escalável, seguro e de baixo custo operacional.

---

## 📺 Demonstração do Processo

<img width="800" alt="Demonstração do Fluxo" src="https://github.com/user-attachments/assets/f44a9c04-9ee9-4469-999f-3fae3550391d" />

*Interface de preenchimento e execução do workflow em tempo real.*

---

## Arquitetura do Workflow

Abaixo está a visualização técnica dos nós configurados no n8n:

<img width="700" alt="Workflow do n8n" src="https://github.com/user-attachments/assets/c61b0701-2331-4f42-8165-1b2ecf353b46" />

</div>

---

##  Diretrizes do Projeto: Eficiência e Baixo Custo

A escolha por não utilizar modelos de linguagem (LLMs) neste projeto foi estratégica. Ao analisar a necessidade real do projeto, identificou-se que a aplicação de IA elevaria os custos operacionais entre **10% e 20%** sem oferecer ganho real de performance para esta tarefa específica.

**Vantagens da abordagem nativa:**
* **Previsibilidade financeira:** Eliminação de gastos com tokens ou assinaturas de terceiros.
* **Integridade de dados:** Erro zero de processamento, sem riscos de alucinações comuns em modelos generativos.
* **Performance:** Menor latência ao utilizar chamadas diretas às APIs do Google.
* **Conformidade:** Processamento de dados alinhado às boas práticas da **LGPD**, mantendo as informações dentro de um ambiente controlado e determinístico.

## Funcionamento Técnico

1. **Entrada de Dados:** Captura de informações via formulário estruturado.
2. **Processamento:** Validação e tratamento de strings no n8n.
3. **Manipulação de Documentos:** Clonagem de um template mestre no Google Docs e substituição de variáveis via API.
4. **Regras de Negócio:** Cálculo automático de validade (5 dias) e geração de identificador único por cliente.
5. **Finalização:** Armazenamento organizado no Google Drive para distribuição imediata pelo vendedor.

---

<div align="center">

**Nota de Privacidade** Todos os dados pessoais exibidos nas mídias deste repositório (como nomes, e-mails e telefones) são **fictícios** e foram gerados apenas para fins de teste e validação de software.

</div>
