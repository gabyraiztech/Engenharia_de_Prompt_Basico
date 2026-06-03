# 🎮 MÓDULO 1 — Scripts das Aulas 01, 02 e 03
**Integrante responsável:** ________________________________
**Tema do módulo:** Fundamentos — como dar ordens para uma IA

> 📌 **Como usar este script:**
> - Abra o notebook da aula no Jupyter antes de começar
> - Leia tudo com calma uma vez antes de gravar
> - Durante a gravação: leia o que está em **[FALE]**, execute o que está em **[EXECUTE]**, mostre o que está em **[MOSTRE]**
> - Não precisa ser perfeito — é normal pausar, respirar e seguir

---

---

# 🎬 AULA 01 — Roles: Quem Manda Aqui?
**Arquivo:** `01-roles.ipynb`
**Tempo estimado:** 14 minutos

## ANTES DE GRAVAR
- Abrir o arquivo `01-roles.ipynb` no Jupyter
- Executar a célula de setup (célula 1) e confirmar que não deu erro
- Ter este script visível em outra janela ou impresso

---

### [00:00] ABERTURA — na câmera (1 min)

**[CÂMERA]** Apareça sorrindo, olhe para a câmera.

**[FALE]**
> "Olá! Seja bem-vindo ao nosso curso de Engenharia de Prompt.
> Sou [seu nome] e essa é a Aula 01.
> Hoje você vai aprender algo que vai mudar completamente como você conversa com uma IA.
> A pergunta que a gente vai responder é: **quando você manda uma mensagem para o ChatGPT ou qualquer IA, quem decide como ela vai responder?**
> A resposta está nos Roles — e é isso que a gente vai ver agora."

---

### [01:00] CONCEITO — compartilhar tela (2 min)

**[MOSTRE]** Compartilhe a tela com o notebook aberto. Role até a célula de markdown com o conceito.

**[FALE]**
> "Antes de codar, preciso te explicar uma coisa simples.
> Quando você usa uma IA, a conversa é dividida em três papéis — em inglês: *roles*.
>
> O **system** é como a ficha de personagem de um RPG. É onde você define quem a IA vai ser — a personalidade dela, as regras que ela precisa seguir.
>
> O **user** é você — o jogador. É quem faz as perguntas e dá as ordens.
>
> O **assistant** é a IA respondendo — o NPC do jogo, dentro do personagem que você definiu.
>
> Sem o system, a IA responde de um jeito genérico. Com o system bem definido, ela vira exatamente o personagem que você criou."

---

### [03:00] SETUP — executar a primeira célula (1 min)

**[MOSTRE]** Role até a primeira célula de código.

**[FALE]**
> "Vamos começar rodando a célula de configuração. Ela importa as bibliotecas e conecta com a API do Groq — que é o serviço que a gente usa para acessar a IA."

**[EXECUTE]** Clique no botão de executar (▶) da primeira célula.

**[FALE]**
> "Se não aparecer nenhum erro, estamos conectados. Ótimo."

---

### [04:00] DEMONSTRAÇÃO 1 — só o role user (3 min)

**[MOSTRE]** Role até a célula da primeira demonstração.

**[FALE]**
> "Nessa primeira demonstração, a gente só usa o role `user` — sem nenhuma instrução de sistema. É o modo mais básico, igual a você digitar no ChatGPT sem nenhuma configuração."

**[EXECUTE]** Execute a célula.

**[FALE]**
> "Viram o resultado? A IA respondeu de um jeito padrão — clara, mas genérica. Sem personalidade específica.
> Agora veja o que acontece quando a gente adiciona o role `system`."

---

### [07:00] DEMONSTRAÇÃO 2 — com role system (3 min)

**[MOSTRE]** Role até a próxima célula de código.

**[FALE]**
> "Agora a gente adiciona o `system`. Eu coloquei aqui: 'Você é um mestre de RPG de fantasia medieval muito dramático. Use termos como nobre viajante e magia.'
> A mesma pergunta — mas agora com a ficha de personagem definida."

**[EXECUTE]** Execute a célula.

**[FALE]**
> "Perceberam a diferença? É a mesma IA, a mesma pergunta. Mas a resposta é completamente diferente porque a gente definiu quem ela deveria ser.
> Isso é o poder do role `system`. É aqui que você cria a personalidade do seu NPC."

---

### [10:00] DEMONSTRAÇÃO 3 — histórico com assistant (2 min)

**[MOSTRE]** Role até a próxima demonstração.

**[FALE]**
> "Agora tem uma coisa importante: a IA tem amnésia. Ela não lembra o que você falou na mensagem anterior.
> Para ela 'lembrar', você precisa passar o histórico completo da conversa.
> É por isso que existe o role `assistant` — você coloca as respostas anteriores da própria IA para ela ter contexto."

**[EXECUTE]** Execute a célula.

**[FALE]**
> "Viram? A IA respondeu levando em conta o que tinha sido dito antes — porque a gente passou o histórico no `assistant`."

---

### [12:00] SEU TURNO (1 min)

**[MOSTRE]** Role até a célula "Seu Turno".

**[FALE]**
> "Agora chegou a hora de vocês tentarem! Procurem a célula com `???` e preencham:
> no `system`, definam a personalidade do NPC de vocês.
> no `user`, façam uma pergunta para ele.
> Depois é só executar e ver o personagem ganhando vida!"

---

### [13:00] ENCERRAMENTO — na câmera (1 min)

**[CÂMERA]** Olhe para a câmera.

**[FALE]**
> "Então é isso! Agora você sabe o que é um role, como definir a personalidade de uma IA e como passar histórico de conversa.
> Na próxima aula, a gente vai aprender a controlar o 'humor' do NPC — se ele vai ser mais previsível ou mais criativo.
> Até lá!"

---
---

# 🎬 AULA 02 — Parâmetros: o Botão de Criatividade do NPC
**Arquivo:** `02-params.ipynb`
**Tempo estimado:** 13 minutos

## ANTES DE GRAVAR
- Abrir o arquivo `02-params.ipynb` no Jupyter
- Executar a célula de setup antes de gravar
- Saber que: **temperature** = criatividade, **top_p** = variedade de palavras

---

### [00:00] ABERTURA — na câmera (1 min)

**[CÂMERA]** Apareça na câmera.

**[FALE]**
> "Olá! Aula 02. Você já sabe criar um NPC com personalidade usando o system prompt.
> Mas imagina: o seu mercador fala exatamente a mesma coisa toda vez que o jogador chega na loja.
> Fica chato, né?
> Hoje você vai aprender a controlar o quanto a IA varia as respostas — usando os parâmetros `temperature` e `top_p`.
> Pensa nisso como o **botão de criatividade** do NPC."

---

### [01:00] CONCEITO — compartilhar tela (2 min)

**[MOSTRE]** Abra o notebook, role até a tabela de conceito.

**[FALE]**
> "Olha essa tabela aqui. O parâmetro `temperature` vai de 0 até 2.
>
> Com **temperature 0**: o NPC é previsível. Ele vai dar sempre a resposta mais óbvia. Como um guarda de fantasia que só fala 'Pode passar' sem variação nenhuma.
>
> Com **temperature 0.7**: equilíbrio. O NPC tem personalidade sem perder o sentido. É o mais usado para NPCs de diálogo normal.
>
> Com **temperature acima de 1**: criativo e imprevisível. Ótimo para oráculos, vilões loucos ou personagens excêntricos. Mas cuidado — pode sair coisa sem sentido.
>
> O `top_p` controla o vocabulário que a IA considera. Baixo = palavras mais comuns. Alto = mais variedade. Na prática, você raramente vai precisar mudar o top_p — foque na temperature."

---

### [03:00] SETUP (30 seg)

**[EXECUTE]** Execute a célula de setup.

**[FALE]** "Setup feito, vamos para a demonstração."

---

### [03:30] DEMONSTRAÇÃO — 3 temperaturas (5 min)

**[MOSTRE]** Role até a célula de demonstração.

**[FALE]**
> "Aqui a gente tem o mesmo NPC — o Oráculo Vel'Zar — respondendo a mesma pergunta com três temperaturas diferentes. Vou executar e a gente vê ao vivo."

**[EXECUTE]** Execute a célula.

**[FALE]** Enquanto os resultados aparecem:
> "Olha a diferença! Com temperature zero, ele respondeu de um jeito direto e seco.
> Com 0.7, tem mais personalidade mas ainda faz sentido.
> Com 1.5... olha só como ficou mais dramático e diferente — é um oráculo de verdade!
> Mesma IA, mesma pergunta. O que mudou foi só o número."

---

### [08:30] DEMONSTRAÇÃO 2 — top_p (2 min)

**[MOSTRE]** Role até a segunda demonstração.

**[FALE]**
> "Agora vou mostrar o top_p rapidinho. Aqui o narrador do jogo descreve a entrada de uma dungeon.
> Com top_p baixo, ele usa palavras mais simples e diretas. Com top_p alto, o vocabulário fica mais variado e poético."

**[EXECUTE]** Execute a célula.

**[FALE]**
> "Sacaram? Para a maioria dos casos do jogo de vocês, mexam na temperature. O top_p deixem padrão."

---

### [10:30] SEU TURNO (1 min)

**[MOSTRE]** Célula Seu Turno.

**[FALE]**
> "Agora testem! Criem um NPC nos `???`, definam uma pergunta e **troquem o número da temperature**. Rodem duas vezes com valores diferentes e vejam como o personagem muda."

---

### [11:30] ENCERRAMENTO — na câmera (1 min)

**[CÂMERA]**

**[FALE]**
> "Agora você sabe controlar o quanto a IA varia. Na próxima aula, a gente vai aprender a escrever prompts muito melhores — porque saber o que pedir faz toda a diferença. Até lá!"

---
---

# 🎬 AULA 03 — Boas Práticas: Quests que a IA Entende
**Arquivo:** `03-boas_praticas.ipynb`
**Tempo estimado:** 14 minutos

## ANTES DE GRAVAR
- Abrir o arquivo `03-boas_praticas.ipynb` no Jupyter
- A aula mostra 4 comparações: vago vs. específico — leia todas antes de gravar

---

### [00:00] ABERTURA — na câmera (1 min)

**[CÂMERA]**

**[FALE]**
> "Aula 03! Você já sabe criar um NPC e controlar a criatividade dele.
> Mas agora surge um problema: você pede para a IA criar uma quest e ela entrega algo genérico demais.
> Por quê? Porque o seu prompt estava vago.
> Hoje a gente aprende **boas práticas de prompt** — como escrever instruções claras para a IA entregar exatamente o que você precisa."

---

### [01:00] CONCEITO (2 min)

**[MOSTRE]** Notebook aberto, rolar até o conceito.

**[FALE]**
> "A regra é simples: escrever um bom prompt é como dar a **ficha de quest** para um narrador de RPG.
>
> Se você chega e diz 'cria uma quest' — o narrador vai inventar qualquer coisa.
>
> Mas se você diz 'cria uma quest de 3 etapas para um ladino nível 5, passando por uma taverna, floresta e castelo, com tom de suspense e sem dragões' — ele vai criar exatamente o que você precisa.
>
> As 4 regras de ouro são:
> **1. Use verbos de ação** — 'crie', 'liste', 'explique'
> **2. Seja específico** — personagem, nível, ambiente, quantidade
> **3. Controle o formato** — tabela? lista? parágrafo?
> **4. Use separadores** quando misturar contexto e instrução"

---

### [03:00] SETUP (30 seg)

**[EXECUTE]** Execute o setup.

---

### [03:30] DEMONSTRAÇÃO 1 — vago vs. específico (3 min)

**[MOSTRE]** Primeira demonstração.

**[FALE]**
> "Vou rodar os dois lados para vocês verem ao vivo. Primeiro o prompt vago: 'Crie uma quest de RPG'. Simples assim."

**[EXECUTE]** Execute e deixe o resultado aparecer.

**[FALE]**
> "Viram? Funcionou, mas é genérico. Poderia ser de qualquer jogo.
> Agora o específico."

**[EXECUTE]** Execute o segundo trecho.

**[FALE]**
> "Completamente diferente, né? Mesma IA. O que mudou foi a qualidade do prompt."

---

### [06:30] DEMONSTRAÇÃO 2 — controlando o formato (2 min)

**[MOSTRE]** Segunda demonstração.

**[FALE]**
> "Agora a gente vê como **controlar o formato**. Sem instrução de formato, a IA decide como apresentar. Com formato definido, ela segue o molde."

**[EXECUTE]** Execute os dois.

**[FALE]**
> "O segundo ficou muito mais limpo e fácil de usar no jogo, né? Uma lista organizada em vez de um parágrafo."

---

### [08:30] DEMONSTRAÇÃO 3 — separadores (2 min)

**[MOSTRE]** Terceira demonstração.

**[FALE]**
> "Por último: separadores. Quando você mistura contexto — tipo a lore do mundo — com a instrução do que fazer, a IA pode se confundir.
> Os separadores `---` deixam claro: até aqui é o contexto. A partir daqui é a tarefa."

**[EXECUTE]** Execute.

**[FALE]**
> "Muito melhor. A IA usou exatamente a lore que a gente passou e criou algo coerente com o mundo."

---

### [10:30] SEU TURNO (1 min)

**[MOSTRE]** Célula Seu Turno.

**[FALE]**
> "Agora o desafio de vocês: transformem o prompt vago `Crie uma missão de RPG` em algo específico. Usem pelo menos uma das 4 regras — personagem, formato, separador. Vai ser bem diferente!"

---

### [11:30] ENCERRAMENTO — na câmera (1 min)

**[CÂMERA]**

**[FALE]**
> "Essas boas práticas valem para qualquer coisa que você for pedir para uma IA — não só jogos. No trabalho, na escola, em qualquer ferramenta de IA, um prompt específico sempre entrega mais.
> Na próxima aula, o Integrante B assume e vai mostrar como controlar o **formato da resposta** — tabelas, listas, JSON... até o inventário do seu personagem! Até lá!"
