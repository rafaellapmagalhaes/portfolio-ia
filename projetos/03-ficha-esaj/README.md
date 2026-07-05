[README.md](https://github.com/user-attachments/files/29674122/README.md)
# 03 — Geração automática de ficha de cliente via ESAJ

## 🎯 O problema

Mesma necessidade do projeto EPROC — coletar dados de processos e gerar a ficha do cliente automaticamente — porém para processos que tramitam no **ESAJ**, sistema do Tribunal de Justiça de São Paulo (TJSP).

O ESAJ tem estrutura e navegação próprias, exigindo uma automação específica adaptada às suas particularidades de telas, campos e comportamento.

---

## 💡 A solução

Automação equivalente ao projeto 02, reescrita para o ESAJ: acessa o sistema, navega pelo processo, extrai as informações com IA e entrega a ficha pronta.

**Lógica do fluxo:**

```
Número do processo (input)
        ↓
  Acesso automatizado ao ESAJ (TJSP)
        ↓
  Navegação adaptada à estrutura do ESAJ
        ↓
  Extração de dados com IA
        ↓
  Estruturação das informações
        ↓
  Ficha do cliente pronta para cadastro
```

**Adaptações específicas para o ESAJ:**
- Estrutura de telas diferente do EPROC e PJE
- Campos e nomenclaturas próprias do TJSP
- Tratamento de variações de layout por tipo de processo
- Lógica de navegação por instâncias

---

## 📊 Resultado

Integrado ao mesmo pipeline dos projetos 02 e 04.  
Os três sistemas juntos (EPROC + ESAJ + PJE) cobrem a grande maioria dos processos trabalhados pelo escritório.

| | Antes | Depois |
|---|---|---|
| Tempo por ficha | ~30–40 min | ~2–3 min |
| Cobertura | Manual e parcial | Automatizada nos 3 sistemas |

---

## 🛠 Stack

- **IA:** Claude (Anthropic)
- **Sistema alvo:** ESAJ (TJSP)
- **Output:** Ficha estruturada (.docx)

---

> ⚠️ O prompt e as instruções internas são proprietários e não estão disponíveis neste repositório.
