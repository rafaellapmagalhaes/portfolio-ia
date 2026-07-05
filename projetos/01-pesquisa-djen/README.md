[README.md](https://github.com/user-attachments/files/29674100/README.md)
# 01 — Pesquisa de processos rentáveis no DJEN

## 🎯 O problema

O escritório precisava monitorar diariamente o Diário da Justiça Eletrônico Nacional (DJEN) para identificar processos com potencial de **cessão de créditos** — uma oportunidade de negócio que exige leitura, interpretação e triagem de um volume muito alto de publicações.

Esse trabalho era feito manualmente por funcionários, consumindo horas do dia sem garantia de consistência ou cobertura total das publicações.

**Situação anterior:**
- Funcionários dedicados lendo publicações manualmente
- Alta chance de perder oportunidades por volume
- Processo cansativo e sujeito a erro humano
- Resultado dependente da atenção e conhecimento de cada pessoa

---

## 💡 A solução

Automação que acessa o DJEN diariamente, lê as publicações relevantes, interpreta o conteúdo com IA e filtra apenas os processos que se enquadram nos critérios de cessão de créditos.

**Lógica do fluxo (sem revelar o prompt):**

```
DJEN (publicações do dia)
        ↓
  Coleta automatizada
        ↓
  Leitura e interpretação pela IA
        ↓
  Filtragem por critérios de cessão de créditos
        ↓
  Lista estruturada de processos rentáveis
        ↓
  Entrega para o time jurídico analisar
```

**O que a IA avalia em cada processo:**
- Tipo de crédito envolvido
- Fase processual
- Perfil das partes
- Indicadores de viabilidade de cessão

---

## 📊 Resultado

| | Antes | Depois |
|---|---|---|
| Quem fazia | Funcionários humanos | IA (100% automatizado) |
| Tempo | Horas por dia | Automático, diariamente |
| Cobertura | Parcial (limitada pela atenção humana) | Total (todas as publicações) |
| Consistência | Variável | Uniforme |

---

## 🛠 Stack

- **IA:** Claude (Anthropic), agora está 100% automatizado por Python, sem uso de IA
- **Fonte:** DJEN (Diário da Justiça Eletrônico Nacional)
- **Output:** Relatório estruturado diário, planilha Excel.

> ⚠️ O prompt e as instruções internas são proprietários e não estão disponíveis neste repositório.
