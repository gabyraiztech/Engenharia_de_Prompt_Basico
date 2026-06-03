# 🎮 MÓDULO 3 — Scripts das Aulas 07, 08 e 09
**Integrante responsável:** ________________________________
**Tema do módulo:** Técnicas — planejamento em etapas e raciocínio da IA

> 📌 **Como usar este script:**
> - Abra o notebook da aula no Jupyter antes de começar
> - Leia tudo com calma uma vez antes de gravar
> - **[FALE]** = diga isso | **[EXECUTE]** = clique ▶ | **[MOSTRE]** = role até esta parte

---

---

# 🎬 AULA 07 — Multi-Step: Construindo a Dungeon Passo a Passo
**Arquivo:** `07-steps.ipynb`
**Tempo estimado:** 13 minutos

## ANTES DE GRAVAR
- Abrir o arquivo `07-steps.ipynb` no Jupyter
- Executar o setup e confirmar que não deu erro
- Conceito central: dar uma metodologia de etapas para a IA seguir, em vez de pedir tudo de uma vez

---

### [00:00] ABERTURA — na câmera (1 min)

**[CÂMERA]** Apareça sorrindo.

**[FALE]**
> "Olá! Sou [seu nome] e começo agora o Módulo 3.
> Você já sabe criar NPCs incríveis. Agora o desafio é criar algo maior — uma dungeon completa.
> O problema é: se você pedir tudo de uma vez, a IA inventa uma bagunça sem estrutura.
> A solução é o **multi-step** — você define os passos e a IA segue a ordem.
> É como um mestre de jogo experiente que planeja cada andar da dungeon antes de revelar ao grupo."

---

### [01:00] CONCEITO (2 min)

**[MOSTRE]** Notebook, role até o conceito.

**[FALE]**
> "A ideia é simples. Em vez de dizer 'cria uma dungeon', você diz:
>
> 'Passo 1: define o tema e o nome.
> Passo 2: cria os 3 andares com ambientes únicos.
> Passo 3: coloca monstros e armadilhas em cada andar.
> Passo 4: esconde tesouros.
> Passo 5: cria o chefe final.'
>
> Cada passo usa o resultado do anterior. O resultado final é muito mais coeso e completo do que se você pedisse tudo de uma vez."

---

### [03:00] SETUP (30 seg)

**[EXECUTE]** Execute o setup.

---

### [03:30] DEMONSTRAÇÃO PRINCIPAL — dungeon em 5 passos (5 min)

**[MOSTRE]** Demonstração principal.

**[FALE]**
> "Aqui eu passo a metodologia de 5 passos no system e peço uma dungeon de tema aquático.
> Veja como a IA vai construindo cada parte antes de passar para a próxima."

**[EXECUTE]** Execute. Aguarde o resultado aparecer.

**[FALE]**
> "Olha que estrutura incrível! Cada passo foi construído sobre o anterior.
> O tema foi definido → os andares foram criados de acordo com o tema → os monstros fazem sentido com o ambiente → os tesouros estão escondidos em lugares coerentes.
>
> Tudo isso só porque a gente deu uma **metodologia** para a IA seguir, não só um pedido genérico."

---

### [08:30] COMPARAÇÃO — single vs. multi-step (2 min)

**[MOSTRE]** Célula de comparação.

**[FALE]**
> "Pra ficar bem claro: aqui está o single-step — pedi 'crie uma dungeon' sem nenhuma metodologia — e o multi-step com os passos definidos. Vou rodar os dois."

**[EXECUTE]** Execute.

**[FALE]**
> "A diferença fala por si. O single-step tem uma ideia ou outra boa, mas é solto. O multi-step é estruturado, completo e utilizável."

---

### [10:30] SEU TURNO (1 min)

**[MOSTRE]** Célula Seu Turno.

**[FALE]**
> "Criem a dungeon de vocês! Definam um tema nos `???` e o nível do grupo. A metodologia já está no system — só executem e vejam o resultado."

---

### [11:30] ENCERRAMENTO — na câmera (1 min)

**[CÂMERA]**

**[FALE]**
> "Multi-step é muito útil para qualquer tarefa complexa — não só dungeons. Sempre que você precisar de um resultado estruturado e grande, pense em quebrar em passos.
> Na próxima aula, a gente vai ver algo diferente: como fazer a IA **raciocinar em voz alta** antes de responder. Até lá!"

---
---

# 🎬 AULA 08 — Chain of Thought: o NPC que Pensa em Voz Alta
**Arquivo:** `08-cot.ipynb`
**Tempo estimado:** 13 minutos

## ANTES DE GRAVAR
- Abrir o arquivo `08-cot.ipynb` no Jupyter
- Executar o setup antes de gravar
- Conceito central: forçar a IA a mostrar o raciocínio passo a passo usando tags como `<pensamento>`

---

### [00:00] ABERTURA — na câmera (1 min)

**[CÂMERA]**

**[FALE]**
> "Aula 08 — Chain of Thought!
> Você tem um NPC sábio que resolve enigmas na dungeon. Mas ele sempre dá a resposta direta, sem explicar como chegou lá.
> Aí o jogador pensa: 'de onde veio isso?'
> Hoje você aprende a fazer o NPC raciocinar em voz alta — como um detetive explicando o caso passo a passo antes de revelar o culpado.
> Em inglês, isso se chama **Chain of Thought**, ou CoT."

---

### [01:00] CONCEITO (2 min)

**[MOSTRE]** Notebook, role até o conceito.

**[FALE]**
> "A diferença é simples.
>
> **Sem CoT**: você pergunta e o NPC responde direto. Tipo: 'Qual alavanca puxar?' → 'A azul.'
>
> **Com CoT**: o NPC pensa em voz alta primeiro. Ele analisa o enigma, considera as opções, identifica pistas — e aí dá a resposta. Tipo: 'Hmm... a inscrição diz que a verdade fica entre duas mentiras. Se a vermelha e a verde são as extremidades... então a azul, no meio, seria a verdade. Puxe a azul.'
>
> Isso deixa o NPC parecer mais inteligente e o jogador entende o raciocínio.
>
> A gente usa tags como `<pensamento>` no system para separar o raciocínio da resposta final."

---

### [03:00] SETUP (30 seg)

**[EXECUTE]** Setup.

---

### [03:30] DEMONSTRAÇÃO 1 — sem CoT vs. com CoT (4 min)

**[MOSTRE]** Primeira demonstração.

**[FALE]**
> "Aqui tem um enigma: três alavancas — vermelha, azul e verde. 'A verdade fica entre duas mentiras.'
> Primeiro sem CoT, depois com CoT. Vamos ver a diferença."

**[EXECUTE]** Execute.

**[FALE]** Enquanto aparece:
> "Sem CoT: respondeu direto. Pode estar certo ou errado, mas não explica o porquê.
>
> Com CoT: olha! Tem o bloco `<pensamento>` onde ele analisou cada possibilidade antes de concluir.
> Como jogador, agora eu entendo a lógica. E como desenvolvedor de jogo, consigo verificar se o NPC está raciocinando certo."

---

### [07:30] DEMONSTRAÇÃO 2 — General Kavros (3 min)

**[MOSTRE]** Segunda demonstração.

**[FALE]**
> "Aqui tem um uso mais prático: um general estratégico que analisa uma batalha.
> O group enfrenta um troll e três arqueiros goblin. O general vai pensar passo a passo antes de sugerir o plano."

**[EXECUTE]** Execute.

**[FALE]**
> "Perfeito! Ele avaliou as forças, identificou os pontos fracos de cada inimigo, calculou riscos e propôs um plano de 3 movimentos.
> Isso é CoT em ação: raciocínio estruturado e transparente."

---

### [10:30] SEU TURNO (1 min)

**[MOSTRE]** Célula Seu Turno.

**[FALE]**
> "Criem um enigma para a dungeon de vocês e usem a célula do Seu Turno. O NPC já está configurado para usar o formato `<pensamento>` — só substituam o enigma nos `???` e executem."

---

### [11:30] ENCERRAMENTO — na câmera (1 min)

**[CÂMERA]**

**[FALE]**
> "CoT é especialmente útil quando você quer que a IA tome decisões, resolva problemas complexos ou justifique escolhas.
> Na próxima aula, a gente vai ver como resumir histórias longas — tipo o log de aventura do herói depois de muitas sessões. Até lá!"

---
---

# 🎬 AULA 09 — Sumarização: O Escriba das Aventuras
**Arquivo:** `09-sumarizacao.ipynb`
**Tempo estimado:** 13 minutos

## ANTES DE GRAVAR
- Abrir o arquivo `09-sumarizacao.ipynb` no Jupyter
- Executar o setup antes de gravar
- Esta aula tem 4 tipos de resumo — leia todos antes de gravar para saber o que esperar de cada um

---

### [00:00] ABERTURA — na câmera (1 min)

**[CÂMERA]**

**[FALE]**
> "Aula 09!
> Depois de muitas sessões de jogo, o log de aventura do herói ficou enorme. 10 sessões de detalhes...
> Ninguém vai querer ler tudo na abertura da próxima sessão.
> Hoje você aprende **sumarização** — pedir para a IA condensar textos longos sem perder o que importa.
> É como ter um escriba que transforma 50 pergaminhos em um relatório de uma página."

---

### [01:00] CONCEITO (2 min)

**[MOSTRE]** Notebook, role até o conceito.

**[FALE]**
> "Sumarização é pedir para a IA reduzir um texto, mantendo as informações mais importantes.
>
> O segredo está no **system prompt**: você define quem é o escriba — e isso muda tudo.
>
> Um narrador épico vai fazer um resumo dramático e heróico.
> Um analista tático vai fazer bullet points secos e diretos.
> O sistema do jogo vai gerar um JSON para salvar no banco de dados.
>
> O mesmo texto, estilos de resumo completamente diferentes — depende de quem você coloca no system."

---

### [03:00] SETUP (30 seg)

**[EXECUTE]** Setup.

---

### [03:30] DEMONSTRAÇÃO 1 — resumo básico (2 min)

**[MOSTRE]** Primeira demonstração — tem o log de aventura da Sessão 7 escrito na variável.

**[FALE]**
> "Aqui está o log da Sessão 7 — cheio de detalhes. O escriba do reino vai resumir para 1/3 do tamanho, preservando os eventos-chave."

**[EXECUTE]** Execute.

**[FALE]**
> "Perfeito — mesmo texto, mas compacto. Todos os eventos importantes estão lá."

---

### [05:30] DEMONSTRAÇÃO 2 — bullet points (1 min)

**[MOSTRE]** Segunda demonstração.

**[FALE]**
> "Agora um analista tático — bullet points organizados por categoria: eventos, itens, estado do grupo, próximos objetivos."

**[EXECUTE]** Execute.

**[FALE]**
> "Ótimo para revisar rapidamente antes de uma sessão."

---

### [06:30] DEMONSTRAÇÃO 3 — abertura épica (1 min)

**[MOSTRE]** Terceira demonstração.

**[FALE]**
> "Agora uma abertura dramática para o início da próxima sessão — como aquelas aberturas de série que resumem o episódio anterior."

**[EXECUTE]** Execute.

**[FALE]**
> "Essa daria para colocar como narração no início de um vídeo!"

---

### [07:30] DEMONSTRAÇÃO 4 — JSON (1 min)

**[MOSTRE]** Quarta demonstração.

**[FALE]**
> "E por último: o estado do jogo em JSON. Para quem está construindo um app, esse formato é perfeito para salvar no banco de dados."

**[EXECUTE]** Execute.

---

### [08:30] SEU TURNO (2 min)

**[MOSTRE]** Célula Seu Turno.

**[FALE]**
> "Criem o log de uma aventura — pode ser de 5 linhas, pode inventar tudo — e escolham um estilo de resumo. Substituam os `???` e executem."

---

### [10:30] ENCERRAMENTO — na câmera (1 min)

**[CÂMERA]**

**[FALE]**
> "Sumarização é super prática — serve para resumir reuniões, artigos, capítulos de livro, qualquer coisa.
> O Módulo 4 começa agora com [nome do Integrante D], que vai fechar o curso com as aulas de texto e o projeto final.
> Até lá e bom jogo!"
