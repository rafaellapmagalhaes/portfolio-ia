[README.md](https://github.com/user-attachments/files/29674116/README.md)
# 02 — Geração automática de ficha de cliente via EPROC

## 🎯 O problema

Após identificar um processo de interesse no DJEN, o próximo passo era acessar o sistema **EPROC**, navegar pelo processo, coletar todas as informações necessárias e montar manualmente a ficha do possível cliente para cadastramento interno.

Esse trabalho era repetitivo, demorado e exigia atenção a muitos campos — nome, CPF/CNPJ, endereço, advogado, valor da causa, fase processual, histórico de movimentações, entre outros.

**Situação anterior:**
- Funcionário acessa o EPROC manualmente
- Copia campo por campo das informações do processo
- Monta a ficha num documento ou sistema interno
- Processo todo feito 1 a 1, processo por processo
- Altíssimo risco de erro ou campo esquecido

---

## 💡 A solução

Automação que recebe o número do processo, acessa o EPROC, navega pelas telas relevantes, extrai todas as informações necessárias e gera a ficha do cliente já formatada e pronta para cadastramento.

**Lógica do fluxo:**

```
Número do processo (input)
        ↓
  Acesso automatizado ao EPROC
        ↓
  Navegação nas telas do processo
        ↓
  Extração de dados com IA
        ↓
  Estruturação das informações
        ↓
  Ficha do cliente pronta para cadastro
```

**Dados extraídos automaticamente:**
- Identificação das partes (autor, réu, advogados)
- CPF / CNPJ
- Endereço quando disponível
- Valor da causa
- Fase e status processual
- Últimas movimentações relevantes
- Informações para análise de cessão

---

## 📊 Resultado

| | Antes | Depois |
|---|---|---|
| Tempo por ficha | ~30–40 min | ~2–3 min |
| Quem fazia | Funcionário dedicado | IA (automatizado) |
| Risco de erro | Alto (manual) | Baixo (estruturado) |
| Volume possível | Limitado pela pessoa | Escalável |

> Este projeto faz parte de um pipeline integrado com os projetos **03 (ESAJ)** e **04 (PJE)**, cobrindo os três principais sistemas judiciais utilizados.

---

## 🛠 Stack

- **IA:** Claude (Anthropic)
- **Automação web:** Playwright
- **Orquestração:** n8n
- **Sistema alvo:** EPROC
- **Output:** Ficha estruturada (JSON / documento)

---

> ⚠️ O prompt e as instruções internas são proprietários e não estão disponíveis neste repositório.
