[README.md](https://github.com/user-attachments/files/29674126/README.md)
# 04 — Geração automática de ficha de cliente via PJE

## 🎯 O problema

Terceiro sistema judicial do pipeline: o **PJE (Processo Judicial Eletrônico)**, utilizado por vários tribunais federais e estaduais. Mesma necessidade — extrair dados do processo e gerar a ficha do cliente — com a complexidade adicional de que o PJE tem comportamentos e estruturas distintos dos outros dois sistemas.

---

## 💡 A solução

Automação desenvolvida especificamente para o PJE, fechando o pipeline de três sistemas (EPROC + ESAJ + PJE) e garantindo cobertura completa independente do tribunal onde o processo tramita.

**Lógica do fluxo:**

```
Número do processo (input)
        ↓
  Identificação automática do tribunal/instância
        ↓
  Acesso ao PJE correto
        ↓
  Navegação e extração de dados
        ↓
  Interpretação com IA
        ↓
  Ficha do cliente pronta para cadastro
```

**Desafios específicos do PJE:**
- Variações de interface por tribunal
- Autenticação e sessão
- Estrutura de dados menos padronizada
- Necessidade de identificar o tribunal correto automaticamente

---

## 📊 Pipeline completo — visão integrada

Os projetos 02, 03 e 04 formam um pipeline unificado:

```
DJEN identifica processo rentável (Projeto 01)
              ↓
   Qual sistema o processo usa?
    ↙         ↓         ↘
EPROC       ESAJ        PJE
(Proj 02)  (Proj 03)  (Proj 04)
    ↘         ↓         ↙
      Ficha do cliente gerada
              ↓
       Cadastro no sistema interno
```

**Resultado do pipeline completo:**
- 5 funcionários fazendo fichas o dia todo → substituído por IA em ~5 horas
- Cobertura dos 3 principais sistemas judiciais
- Fichas padronizadas e sem erro de digitação

---

## 🛠 Stack

- **IA:** Claude (Anthropic)
- **Sistema alvo:** PJE
- **Output:** Ficha estruturada (.docx)

---

> ⚠️ O prompt e as instruções internas são proprietários e não estão disponíveis neste repositório.
