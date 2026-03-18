---
description: Pesquisa um tema na web (notícias, artigos científicos, trends) e gera um roteiro completo para YouTube focado em retenção.
---

Este workflow automatiza a pesquisa e criação de roteiros para o YouTube, garantindo rigor científico, dados atualizados e uma estrutura narrativa cativante.

# Passos do Agente Roteirista

1. Entender o Tema

Capture o tema ou palavra-chave fornecido pelo usuário.

Defina também:
	•	público-alvo provável
	•	principais dúvidas relacionadas
	•	crenças erradas comuns sobre o tema

⸻

2. Pesquisa Estratégica na Web

Utilize search_web para buscar:
	•	artigos e notícias recentes
	•	estudos científicos atualizados
	•	estatísticas relevantes
	•	tendências sociais/comportamentais ligadas ao tema

Priorize:
	•	revisões sistemáticas
	•	meta-análises
	•	instituições confiáveis

Evite fontes fracas ou sensacionalistas.

⸻

3. Síntese Estratégica

Organize a pesquisa em:
	•	1 dado chocante ou contraintuitivo
	•	crenças erradas comuns
	•	principais dores do público
	•	explicação científica central
	•	soluções práticas baseadas em evidências

Traduza conceitos complexos para linguagem simples e acessível.

⸻

4. Escrita do Roteiro (Com Retenção)

Ative ativamente a skill `Caçador de Retenção` (cacador_de_retencao) durante a redação do roteiro para aplicar rigorosamente as técnicas de "Open Loops", "Re-hooks" e ganchos de alta retenção.

[0:00 – 0:30] HOOK

Crie 3 versões:
	1.	quebra de crença
	2.	pergunta provocativa
	3.	frase direta

Inclua:
	•	sugestão visual
	•	cortes
	•	texto na tela
	•	ritmo rápido

⸻

[0:30 – 2:00] O PROBLEMA
	•	forte identificação emocional
	•	exemplos do cotidiano
	•	micro-narrativas

Inclua:
	•	perguntas ao espectador
	•	pausas estratégicas

⸻

[2:00 – 5:00] A CIÊNCIA
	•	explicação clara e didática
	•	analogias
	•	exemplos práticos
	•	sem linguagem acadêmica

Inclua:
	•	gráficos
	•	ilustrações
	•	mudanças de ritmo

A cada ~60s inserir elemento de retenção.

⸻

[5:00 – 7:00] A SOLUÇÃO
	•	passos acionáveis
	•	simples
	•	realistas
	•	sem promessas irreais

⸻

[7:00 – 8:00] CTA
	•	reflexão final
	•	pergunta aberta
	•	convite natural

Evitar CTA genérico.

⸻

5. Referências

Ao final do roteiro, liste os links e fontes reais que você encontrou na Etapa 2 para que o criador de conteúdo tenha segurança no que está falando.
**Atenção aos Links Essenciais:** Não é obrigatório incluir todas as referências. É OBRIGATÓRIO fornecer os links exatos de onde foram extraídos **dados de pesquisas, estatísticas (ex: "30% dos americanos estão com diabetes antes dos 30"), páginas com gráficos e notícias**. Isso é fundamental para que o usuário possa acessar o site e tirar prints da tela para colocar no vídeo.

⸻

6. Validação Científica

Usando os critérios da skill `Validação Científica` (validador_cientifico), analise o roteiro recém-criado marcando afirmações questionáveis com [FATO VERIFICADO], [FATO PARCIAL / NECESSITA CUIDADO] ou [MITO / REMOVER], e ajuste o tom do texto.

⸻

7. Títulos e Thumbnails

Ative a skill `Especialista em Títulos e Thumbnails do YouTube` (metadados_youtube) para avaliar o roteiro criado. Siga fielmente as regras da skill, gerando 5 opções de títulos magnéticos e 2 direcionamentos visuais de thumbnail para cada opção.

⸻

8. Derivação de Conteúdo

Ative a skill `Derivação de Conteúdo` (derivacao_de_conteudo) para ler o roteiro longo aprovado, extraindo e gerando 3 roteiros virais e curtos adaptados para TikTok/Reels/Shorts, cada um em base na "Caça aos Gold Nuggets".

⸻

9. Formatação Visual do Roteiro

Ative a skill `Formatador de Roteiro Visual` (formatador_de_roteiro) para revisar todo o conteúdo textual gerado nos passos anteriores, aplicando rigorosamente as regras de espaçamento, emojis, marcação visual (`[B-ROLL]`) e blocos de citação (`> `) estabelecidas para facilitar muito a leitura final e teleprompter.

⸻

10. Exibir Resultado na Tela

Gere o resultado final formatado como um artifact (usando a ferramenta `write_to_file` com `IsArtifact: true`), para que ele seja aberto diretamente na tela do usuário para visualização e edição. O próprio usuário salvará o arquivo na pasta de roteiros posteriormente.

O arquivo gerado deve conter todo o conteúdo estritamente na seguinte ordem, com separadores visuais claros entre as seções:

1. **# [Roteiro Longo]** — O roteiro completo com as referências, validação científica e sugestões de Títulos/Thumbnails.
2. **# [Shorts]** — Os 3 roteiros curtos extraídos pela Derivação de Conteúdo.

Após gerar o artifact, envie uma mensagem curta no chat informando que o roteiro está pronto para revisão e salvamento.