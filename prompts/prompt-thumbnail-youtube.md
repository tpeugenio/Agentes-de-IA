# Prompt de thumbnail — O Peso da Mente (Nano Banana 2)

## Como usar (rápido)

1. Preencha **todos os campos editáveis** abaixo (não envie com chaves vazias).
2. Copie o **Prompt final** completo e cole no gerador de imagens (ex.: Gemini / Nano Banana 2).
3. Peça **proporção 16:9** e, se a interface permitir, **1920×1080** ou **4K 16:9**.
4. Gere **duas variações** (A minimal / B com mais cor) usando a seção opcional, se quiser comparar rápido.
5. Se o texto sair fraco, use uma **frase de refinamento** da seção final — sem mudar o texto exato da thumbnail.

---

## Campos editáveis (preencher antes de cada vídeo)

Copie esta tabela para seu rascunho ou preencha inline.

| Campo | Seu conteúdo |
|--------|----------------|
| **{{TEMA}}** | |
| **{{RESUMO}}** | 2–4 frases: o que o vídeo aborda |
| **{{TEXTO_NA_THUMB}}** | Texto **exato** em português na imagem (3–7 palavras) |
| **{{OBJETOS_E_ESTILO}}** | Objetos, metáforas, cenário; estilo (foto leve, ilustração flat, editorial, etc.) |
| **{{TOM}}** | Tom emocional (acolhimento, esperança calma, curiosidade, etc.) |
| **{{RESTRIÇÕES}}** | Ex.: sem rosto, sem marcas, público-alvo, evitar X |
| **{{PUBLICO_ALVO}}** *(opcional)* | Ex.: jovens adultos, +40, estudantes |
| **{{COR_DESTAQUE}}** *(opcional)* | Uma cor ou hex, ex.: `#4A6FA5` |

---

## Bloco FIXO — identidade do canal (revisar só de tempos em tempos)

Use sempre junto com o prompt principal. Ajuste **paleta** quando tiver cores oficiais do canal.

- **Canal:** O Peso da Mente — YouTube sobre **saúde mental**: informação séria, linguagem acessível, **sem sensacionalismo** nem clickbait agressivo.
- **Tom de marca:** profissional, humano, respeitoso; convida à reflexão sem ridicularizar ou estigmatizar.
- **Paleta sugerida (editável):** tons suaves e legíveis; bom contraste entre texto e fundo. *(Substitua por primária/secundária oficiais quando existirem, ex.: primária `#______`, secundária `#______`.)*

---

## Especificação técnica — Nano Banana 2 / thumbnail YouTube

Inclua **sempre** no início ou no fim do prompt (a interface pode aceitar proporção em campo separado — use os dois se disponível):

- **Formato:** thumbnail para YouTube, **proporção 16:9**, **alta resolução** (ideal **1920×1080**; se a ferramenta oferecer, **4K 16:9**).
- **Legibilidade:** composição pensada para **tela pequena** (celular); texto grande, **área segura** central e laterais sem elementos críticos nos cantos extremos.
- **Texto em português:** renderizar **exatamente** o texto fornecido em `{{TEXTO_NA_THUMB}}`, tipografia **sans-serif bold**, **alto contraste** (fundo escuro + texto claro, ou o inverso), **contorno fino ou sombra suave** para leitura.
- **Hierarquia:** um foco visual principal (rosto, objeto ou forma) + título dominante; evitar poluição visual.

---

## Prompt master (copiar, preencher placeholders e enviar)

```
[FORMATO] Thumbnail YouTube 16:9, alta resolução (1920x1080 ou 4K 16:9 se disponível), otimizada para leitura em tela pequena, estilo profissional para canal de saúde mental em português (Brasil).

[CONTEÚDO DO VÍDEO]
Tema: {{TEMA}}
Resumo do que é falado: {{RESUMO}}

[TEXTO NA IMAGEM — PORTUGUÊS]
Incluir na arte, com ortografia exata e legível: "{{TEXTO_NA_THUMB}}"

[VISUAL]
Elementos, metáforas e estilo desejados: {{OBJETOS_E_ESTILO}}
Tom emocional da arte: {{TOM}}
Restrições específicas deste vídeo: {{RESTRIÇÕES}}
Público-alvo (se informado): {{PUBLICO_ALVO}}
Cor de destaque (se informada): {{COR_DESTAQUE}}

[IDENTIDADE — O PESO DA MENTE]
Canal sobre saúde mental: informação séria e acessível, acolhedora, sem sensacionalismo. Evitar clickbait visual agressivo. Composição limpa, contraste alto entre texto e fundo, área segura para título (evitar cortar texto nos cantos no mobile).

[NEGATIVO — NÃO INCLUIR]
Violência explícita, automutilação, drogas em destaque sensacionalista, gore, estereótipos de "loucura" ou manicômicos, imagens humilhantes ou degradantes, distorção facial exagerada só para chamar atenção, texto ilegível ou errado, marcas/logos de terceiros, watermark falso, conteúdo infantilizado que minimize sofrimento psíquico.
```

---

## Checklist antes de gerar

- [ ] `{{TEXTO_NA_THUMB}}` está **curto**, **sem erro** de ortografia e é o título que você quer publicar.
- [ ] `{{RESUMO}}` dá contexto suficiente para metáforas adequadas (sem pedir imagens gráficas de sofrimento).
- [ ] Proporção **16:9** e foco em **legibilidade mobile** estão pedidos.
- [ ] Tom condiz com **saúde mental** (respeito, sem estigma).
- [ ] Se usar rosto gerado, está ok para o tema; caso contrário, `{{RESTRIÇÕES}}` pede “sem rosto” ou “silhueta abstrata”.

---

## Opcional — duas variações na mesma rodada

Se a ferramenta permitir duas imagens ou dois prompts seguidos, use o mesmo conteúdo acima e acrescente **só uma linha** ao final:

- **Variação A:** “Versão mais minimalista: menos elementos, mais espaço negativo, texto ainda mais dominante.”
- **Variação B:** “Versão com mais cor e profundidade atmosférica, mantendo o mesmo texto em português e a mesma hierarquia.”

---

## Frases de refinamento (segunda iteração, sem mudar o título)

Use quando a primeira imagem estiver boa, mas faltar punch ou legibilidade:

1. “Manter **exatamente** o texto em português: `{{TEXTO_NA_THUMB}}`. Aumentar contraste entre texto e fundo; simplificar o fundo.”
2. “Reduzir elementos secundários; deixar um único foco visual + o título.”
3. “Texto um pouco maior na composição; sombra ou contorno mais visível nas letras.”
4. “Paleta mais coesa; menos cores competindo com o título.”
5. “Manter tom acolhedor; menos saturação agressiva; nada de expressão facial exagerada.”

---

## Exemplo preenchido (referência)

| Campo | Exemplo |
|--------|---------|
| {{TEMA}} | Ansiedade no trabalho |
| {{RESUMO}} | O vídeo explica sinais de ansiedade no ambiente laboral, pausas curtas e como conversar com liderança sem se culpar. |
| {{TEXTO_NA_THUMB}} | ANSIEDADE NO TRABALHO |
| {{OBJETOS_E_ESTILO}} | Mesa de escritório suave ao fundo, planta pequena, luz de janela; estilo editorial limpo, levemente fotorealista |
| {{TOM}} | Acolhimento e clareza, sem alarmismo |
| {{RESTRIÇÕES}} | Sem rosto identificável; sem logos de empresas |
| {{PUBLICO_ALVO}} | Adultos em ambiente corporativo |
| {{COR_DESTAQUE}} | Azul-acinzentado suave `#5B7C99` |

---

*Documento gerado para o canal **O Peso da Mente** e uso com **Nano Banana 2** (ou equivalente com texto em imagem e 16:9). Atualize o bloco de paleta quando a identidade visual oficial estiver definida.*
