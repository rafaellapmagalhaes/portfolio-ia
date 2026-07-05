[README.md](https://github.com/user-attachments/files/29674131/README.md)
# 05 — Automação completa de redes sociais (Instagram)

## 🎯 O problema

A produção de conteúdo para o Instagram do escritório era feita completamente de forma manual: pensar nos temas, escrever as legendas, criar as artes, revisar, aprovar e agendar. Um processo que envolvia múltiplas pessoas e tomava **uma semana inteira** para entregar os posts da semana.

**Situação anterior:**
- Reunião de pauta para definir temas
- Redação de legendas por uma pessoa
- Criação de arte por outra
- Rodadas de revisão e aprovação
- Agendamento manual
- **Tempo total: ~1 semana por ciclo de posts**

---

## 💡 A solução

Pipeline de IA que assume todo o processo de produção de conteúdo — da ideia à publicação — de forma autônoma. A IA define os temas relevantes, cria as legendas, gera as imagens e publica no Instagram.

**Lógica do fluxo:**

```
Briefing / diretrizes da empresa (input único)
        ↓
  IA gera pauta de conteúdos da semana
        ↓
  Para cada post:
    ├── Criação da legenda (tom, CTA, hashtags)
    ├── Geração da imagem / arte visual
    └── Revisão interna automatizada
        ↓
  Agendamento e publicação no Instagram
        ↓
  Relatório do que foi publicado
```

**O que a IA faz em cada post:**
- Define tema alinhado ao nicho jurídico
- Escreve legenda no tom da marca
- Seleciona e adapta hashtags relevantes
- Gera imagem com identidade visual consistente
- Valida antes de publicar
- Agenda no horário de maior engajamento

---

## 📊 Resultado

| | Antes | Depois |
|---|---|---|
| Pessoas envolvidas | 2–3 (redator, designer, aprovador) | 0 (100% automatizado) |
| Tempo de produção | ~1 semana | ~1 dia |
| Consistência visual | Variável | Padronizada |
| Volume possível | Limitado | Escalável |

---

## 🖼 Exemplo de output (fictício)

**Post gerado automaticamente:**

> 📋 **Legenda:**  
> Você sabia que é possível monetizar créditos judiciais mesmo sem ser advogado?  
> A cessão de créditos permite que terceiros adquiram o direito ao recebimento de valores devidos por decisão judicial.  
> Quer entender como isso funciona? Fala com a gente. 👇  
> #cessãodecreditos #direitojuridico #advogado #processosjudiciais

**Arte:** Gerada com identidade visual do escritório (cores, tipografia, logo).

---

## 🛠 Stack

- **IA de texto:** Claude (Anthropic)
- **IA de imagem:** ChatGPT e Claude Design
- **Publicação:** Instagram Graph API com Metricool
- **Agendamento:** Integrado via API pelo Metricool

---

> ⚠️ O prompt, as diretrizes de marca e as instruções internas são proprietários e não estão disponíveis neste repositório.
