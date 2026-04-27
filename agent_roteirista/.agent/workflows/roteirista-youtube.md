---
description: Pesquisa um tema na web (notícias, artigos científicos, trends) e gera um roteiro completo para YouTube focado em retenção.
---

Este workflow automatiza a pesquisa e criação de roteiros para o YouTube, priorizando uma narrativa leve, simples e identificável, com humor natural e exemplos do cotidiano. A ciência entra como suporte (cerca de 30% do roteiro), não como protagonista.

# Diretriz de Tom (LEIA ANTES DE TUDO)

O roteiro deve soar como uma conversa entre amigos no bar — não como uma palestra de universidade.

Regras de ouro:
- **70% narrativa, exemplos reais, humor / 30% ciência e dados** (não inverta essa proporção).
- Use **histórias do cotidiano** que qualquer pessoa já viveu (a fila do mercado, o grupo da família no WhatsApp, a segunda-feira, etc.).
- Insira **piadas leves, ironias, comentários espontâneos** — soltar a mão, não ter medo de ser engraçado.
- Trate o espectador como amigo: "tu já passou por isso?", "sabe quando…", "olha que loucura".
- **Evite jargão**. Se aparecer um termo técnico, traduza na hora com analogia simples.
- Dados e estudos só entram quando **realmente fortalecem o ponto** — não para inflar autoridade.
- Limite a no máximo **2-3 estatísticas por roteiro inteiro**. O resto é história, exemplo e sensação.

# Passos do Agente Roteirista

1. Entender o Tema

Capture o tema ou palavra-chave fornecido pelo usuário.

Defina também:
	•	público-alvo provável
	•	principais dúvidas relacionadas
	•	crenças erradas comuns sobre o tema

⸻

2. Pesquisa Estratégica na Web

Utilize search_web para buscar (em ordem de prioridade):
	1.	**histórias reais, casos virais, situações do cotidiano** ligadas ao tema (fórum, Reddit, comentários, redes sociais)
	2.	tendências sociais/comportamentais e memes ligados ao tema
	3.	notícias recentes com personagens humanos (não só números)
	4.	1 ou 2 estudos científicos sólidos (revisões sistemáticas, meta-análises) só para ancorar o ponto principal
	5.	estatísticas — escolha no máximo 2-3 que sejam **chocantes ou contraintuitivas** (não empilhe dados)

Evite fontes fracas ou sensacionalistas, mas **não confunda "rigor" com "academicismo"** — uma boa história do cotidiano vale mais do que 5 estudos no roteiro final.

⸻

3. Síntese Estratégica

Organize a pesquisa em:
	•	1 história / cena do cotidiano forte para abrir
	•	2-3 exemplos reais identificáveis (situações que o público já viveu)
	•	crenças erradas comuns (em linguagem de bar, não de paper)
	•	principais dores do público (com humor onde couber)
	•	1 dado chocante ou contraintuitivo (só 1, escolha o melhor)
	•	explicação central simplificada via **analogia do dia a dia**
	•	soluções práticas, leves e realistas
	•	2-3 oportunidades de **piada / comentário espontâneo / ironia** durante o roteiro

Traduza qualquer conceito técnico para linguagem de conversa de mesa de bar.

⸻

4. Escrita do Roteiro (Com Retenção)

Ative ativamente a skill `Caçador de Retenção` (cacador_de_retencao) durante a redação do roteiro para aplicar rigorosamente as técnicas de "Open Loops", "Re-hooks" e ganchos de alta retenção.

**Importante:** o resultado deve conter APENAS o texto falado, organizado pelos blocos abaixo (HOOK, PROBLEMA, etc.). **Não inclua sugestões de edição, cortes, B-ROLL, texto na tela, gráficos, pausas dramáticas, sugestões visuais, indicações de ritmo ou qualquer marcação de produção.** A edição é simples e não precisa desses detalhes — apenas o roteiro escrito.

[0:00 – 0:30] HOOK

Crie 3 versões:
	1.	quebra de crença
	2.	pergunta provocativa
	3.	frase direta

⸻

[0:30 – 2:00] O PROBLEMA (com história e humor)
	•	abra com uma **micro-narrativa real** ("sabe quando você…", "ano passado um amigo meu…")
	•	use 2-3 exemplos do cotidiano que o público já viveu
	•	**solte pelo menos 1 piada ou comentário irônico** aqui — naturalidade acima de tudo
	•	identificação emocional vem da história, não do dado
	•	faça perguntas diretas ao espectador

⸻

[2:00 – 5:00] A EXPLICAÇÃO (a "ciência" sem cara de aula)
	•	explique o "porquê" como se estivesse contando pro amigo no bar
	•	**use analogias do dia a dia** (carro, geladeira, WhatsApp, fila do banco) em vez de termos técnicos
	•	**no máximo 1-2 menções a estudos** — e quando mencionar, sem nome de revista científica, só "uma pesquisa de Harvard" ou "um estudo grande mostrou que…"
	•	encaixe **mais 1 piada ou comentário espontâneo** no meio para quebrar o ritmo
	•	exemplos práticos > conceitos abstratos
	•	a cada ~60s insira um elemento textual de retenção (gancho, piada, virada, pergunta) — sempre no próprio texto falado, sem marcações de edição

⸻

[5:00 – 7:00] A SOLUÇÃO (leve e aplicável)
	•	passos acionáveis, simples, realistas
	•	apresente como dica de amigo, não como prescrição médica
	•	tudo bem ter humor aqui também ("não, você não precisa virar monge")
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

**Importante:** a validação serve para garantir que nada do que é afirmado é falso — **não** para transformar o roteiro em paper acadêmico. Se uma afirmação precisar ser suavizada, prefira reescrever em tom de conversa ("parece que…", "tem gente estudando isso e…") em vez de empilhar ressalvas técnicas que matam o ritmo.

⸻

7. Títulos, Thumbnails e Descrição

Ative a skill `Especialista em Títulos, Thumbnails e Descrições do YouTube` (metadados_youtube) para avaliar o roteiro criado. Siga fielmente as regras da skill, gerando 5 opções de títulos magnéticos, 2 direcionamentos visuais de thumbnail para cada opção, além de uma descrição completa com 3 hashtags no final.

⸻

8. Derivação de Conteúdo

Ative a skill `Derivação de Conteúdo` (derivacao_de_conteudo) para ler o roteiro longo aprovado, extraindo e gerando 3 roteiros virais e curtos adaptados para TikTok/Reels/Shorts, cada um em base na "Caça aos Gold Nuggets".

⸻

9. Formatação Visual do Roteiro

Ative a skill `Formatador de Roteiro Visual` (formatador_de_roteiro) para revisar todo o conteúdo textual gerado nos passos anteriores, aplicando as regras de **espaçamento e legibilidade para teleprompter**.

**Não aplicar** marcações de produção como `[B-ROLL]`, indicações de cortes, sugestões visuais ou blocos `> ` de citação cinematográfica. O foco é apenas deixar o texto falado limpo e fácil de ler em voz alta — a edição do vídeo é simples e não usa essas marcações.

⸻

10. Exibir Resultado na Tela

Gere o resultado final como um PDF utilizando a skill `pdf`.

O PDF gerado deve conter todo o conteúdo estritamente na seguinte ordem, com separadores visuais claros entre as seções:

1. **# [Roteiro Longo]** — O roteiro completo com as referências, validação científica e sugestões de Títulos/Thumbnails/Descrição.
2. **# [Shorts]** — Os 3 roteiros curtos extraídos pela Derivação de Conteúdo.

Após gerar o PDF, envie uma mensagem curta no chat informando que o roteiro está pronto para revisão e salvamento.