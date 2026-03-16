---
name: gerador_de_teleprompter
description: Utilizado para gerar um texto limpo no formato teleprompter a partir de um roteiro de gravação. Use esta skill sempre que o usuário pedir para "gerar a versão para teleprompter", "preparar para gravação", "gerar teleprompter do roteiro" ou quando quiser remover indicações de cena e câmera de um roteiro (transformar para leitura fina).
---

# Gerador de Teleprompter

Esta skill ajuda a converter um roteiro de gravação longo e com marcações técnicas (câmera, efeitos, B-roll, textos na tela) em um texto limpo, direto e formatado para ser lido em um aplicativo/software de teleprompter por um apresentador.

## Instruções de Conversão

Ao processar um roteiro, siga RIGOROSAMENTE as seguintes etapas:

1. **Limpeza de Direção e Câmera:** Remova silenciosamente TODA E QUALQUER instrução de direção. Isso inclui cenários, posições de câmera, instruções de edição, B-rolls e legendas que não são faladas.
   - *Eliminar itens como*: `[CÂMERA PRÓXIMA]`, `[ZOOM OUT]`, `[TEXTO NA TELA: ...]`, `[B-ROLL]`, `[EFEITO SONORO]`, `[HOOK]`, `[CORTE RÁPIDO]`, `[OPEN LOOP]`, e as marcações de tempo (ex., `0:00 - 0:30`).

2. **Manutenção Exclusiva das Falas:** Mantenha **APENAS** o texto que será declamado pelo apresentador. Não deve sobrar absolutamente nada no texto que não seja para ser lido em voz alta.

3. **Inclusão de Respiros e Pausas:** Preserve ou traduza inteligentemente as marcações de pausa para que o apresentador saiba onde respirar ou dar entonação.
   - Utilize a marcação `[PAUSA]` (em letras maiúsculas) onde o roteiro sugerir `[PAUSA DE 1 SEGUNDO]`, `[PAUSA DRAMÁTICA]`, ou entre transições de raciocínio.

4. **Formatação de Teleprompter:**
   - Converta para formato `.txt`.
   - Remova tags de Markdown (como `#`, `##`, `**negrito**`, `*itálico*`, `>` de citação).
   - Use quebras de linha frequentes (pule uma linha entre cada frase/período curto). Um texto de teleprompter não pode ter blocos densos; as frases devem ser lidas quase individualmente.

5. **Salvando o Arquivo:**
   - Emita o resultado num arquivo de formato puro de texto `.txt`.
   - Padrão de nome sugerido: `[nome_do_arquivo_original]-teleprompter.txt`.

## Exemplo de Transformação

**Entrada (Roteiro):**
> [CÂMERA PRÓXIMA NO ROSTO, CORTE RÁPIDO A CADA FRASE]
> 
> "Eu tenho uma notícia ruim pra você."
> 
> `[PAUSA DE 1 SEGUNDO]`
> 
> "As redes sociais fizeram você acreditar que você tem um transtorno que talvez você não tenha."
> 
> `[CORTE RÁPIDO | ZOOM OUT]`

**Saída (Teleprompter txt):**
Eu tenho uma notícia ruim pra você.

[PAUSA]

As redes sociais fizeram você acreditar que você tem um transtorno que talvez você não tenha.
