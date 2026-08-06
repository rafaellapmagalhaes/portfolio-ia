# 06 — Resolução automática de CAPTCHAs de texto distorcido

## 🎯 O problema

Diversas automações que acessam certos sites encontram **CAPTCHAs de texto distorcido** como barreira — imagens com letras e números propositalmente embaralhados, inclinados ou com ruído visual, projetados para bloquear robôs.

Esse tipo de bloqueio interrompia o fluxo das automações, exigindo intervenção humana para continuar — quebrando o conceito de automação total.

**Situação anterior:**
- Automação trava ao encontrar um CAPTCHA
- Alguém precisa resolver manualmente para continuar
- Processo deixa de ser 100% autônomo
- Escalabilidade comprometida

---

## 💡 A solução

Sistema desenvolvido em Python que interpreta a imagem do CAPTCHA, lê o texto distorcido e devolve a resposta correta — permitindo que as automações continuem sem interrupção humana.

**Lógica do fluxo:**

```
Automação encontra CAPTCHA na página
        ↓
  Imagem do CAPTCHA é capturada
        ↓
  Sistema Python processa a imagem
        ↓
  Texto distorcido é interpretado
        ↓
  Resposta enviada automaticamente
        ↓
  Automação continua sem interrupção
```

---

## 📊 Resultado

| | Antes | Depois |
|---|---|---|
| O que acontecia ao encontrar CAPTCHA | Automação parava | Continua automaticamente |
| Intervenção humana necessária | Sim | Não |
| Impacto nas automações | Quebrava o fluxo | Zero interrupção |

> Este projeto atua como uma camada de suporte para os demais projetos do portfólio, garantindo que nenhuma automação seja bloqueada por CAPTCHAs.

---

## 🛠 Stack

- **Linguagem:** Python
- **Integração:** Conectado ao pipeline das demais automações

---

> ⚠️ O código e a lógica interna são proprietários e não estão disponíveis neste repositório.
