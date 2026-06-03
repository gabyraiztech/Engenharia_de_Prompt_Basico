# 🎮 MÓDULO 4 — Scripts das Aulas 10, 11, 12 e Projeto Final
**Integrante responsável:** ________________________________
**Tema do módulo:** Aplicações — texto, narrativa e construção do RPG completo

> 📌 **Como usar este script:**
> - Abra o notebook da aula no Jupyter antes de começar
> - Leia tudo com calma uma vez antes de gravar
> - **[FALE]** = diga isso | **[EXECUTE]** = clique ▶ | **[MOSTRE]** = role até esta parte
>
> ⚠️ **Este módulo tem 4 aulas. Se preferir, divida com outro integrante:**
> - Uma pessoa grava as Aulas 10 e 11
> - Outra pessoa grava a Aula 12 e o Projeto Final

---

---

# 🎬 AULA 10 — Complemento de Texto: o Bardo que Continua a História
**Arquivo:** `10-texto_complemento.ipynb`
**Tempo estimado:** 13 minutos

## ANTES DE GRAVAR
- Abrir o arquivo `10-texto_complemento.ipynb` no Jupyter
- Executar o setup antes de gravar
- Conceito central: você dá o início de um texto e a IA continua no mesmo estilo

---

### [00:00] ABERTURA — na câmera (1 min)

**[CÂMERA]** Apareça sorrindo.

**[FALE]**
> "Olá! Sou [seu nome] e começo agora o último módulo do curso.
> Você está escrevendo a lenda de um herói do seu mundo. Começou bem, mas na metade travou.
> Hoje a IA vai ser o seu **bardo particular** — você dá o início e ela continua no mesmo tom, no mesmo estilo.
> Isso se chama text completion, ou complemento de texto."

---

### [01:00] CONCEITO (2 min)

**[MOSTRE]** Notebook, role até o conceito.

**[FALE]**
> "A ideia é: você escreve as primeiras linhas estabelecendo o estilo — épico, sombrio, cômico, poético — e a IA continua a partir do ponto onde você parou.
>
> O contexto do início molda tudo que vem depois. Se você começa em prosa medieval poética, ela continua em prosa medieval poética.
>
> Hoje a gente vai: continuar uma lenda épica, expandir a descrição de uma cidade inteira a partir de uma linha, e criar a lore completa de um item mágico."

---

### [03:00] SETUP (30 seg)

**[EXECUTE]** Execute o setup.

---

### [03:30] DEMONSTRAÇÃO 1 — continuando uma lenda (3 min)

**[MOSTRE]** Primeira demonstração — a variável `lenda_inicio` já tem o texto.

**[FALE]**
> "Aqui está o início de uma lenda épica sobre 7 espadas criadas por um ferreiro divino.
> O texto para na sétima espada e deixa no ar...
> Veja o que o bardo faz com isso."

**[EXECUTE]** Execute.

**[FALE]**
> "Olha o resultado! Ele manteve o tom, a estrutura, o ritmo — continuou como se fosse o mesmo autor.
> E agora tem uma lenda completa para o seu mundo."

---

### [06:30] DEMONSTRAÇÃO 2 — expandindo uma cidade (1 min)

**[MOSTRE]** Segunda demonstração.

**[FALE]**
> "Agora só uma linha sobre uma cidade — e o narrador expande com arquitetura, clima e segredos."

**[EXECUTE]** Execute rapidamente.

**[FALE]**
> "De uma linha para um parágrafo rico. Útil para criar o guia do mundo do jogo."

---

### [07:30] DEMONSTRAÇÃO 3 — lore de item (2 min)

**[MOSTRE]** Terceira demonstração.

**[FALE]**
> "Por último: um item com nome, tipo e poder. A gente pede a lore completa: quem criou, por quê, onde foi perdido e quem o procura agora."

**[EXECUTE]** Execute.

**[FALE]**
> "Cada item do seu mundo pode ter uma história assim. E você não precisa escrever do zero — só definir as características básicas e deixar a IA preencher."

---

### [09:30] SEU TURNO (2 min)

**[MOSTRE]** Célula Seu Turno.

**[FALE]**
> "Escrevam o começo de algo do mundo de vocês — pode ser uma lenda, a descrição de uma cidade ou a origem de um item. A IA vai continuar.
> Substituam os `???` e executem."

---

### [11:30] ENCERRAMENTO — na câmera (1 min)

**[CÂMERA]**

**[FALE]**
> "Text completion é muito útil para escritores e criadores de mundos. Você coloca a direção e a IA expande.
> Na próxima aula, você aprende a pegar esse mesmo texto e adaptar para públicos completamente diferentes. Até lá!"

---
---

# 🎬 AULA 11 — Transformação de Texto: o Mesmo Jogo para Qualquer Público
**Arquivo:** `11-transformacao_texto.ipynb`
**Tempo estimado:** 13 minutos

## ANTES DE GRAVAR
- Abrir o arquivo `11-transformacao_texto.ipynb` no Jupyter
- Executar o setup antes de gravar
- Conceito central: mudar formato, tom ou público do mesmo texto sem perder o conteúdo

---

### [00:00] ABERTURA — na câmera (1 min)

**[CÂMERA]**

**[FALE]**
> "Aula 11!
> Você criou uma quest épica para adultos. Agora o professor quer que você apresente para uma turma de crianças.
> Ou você quer postar nas redes sociais de um jeito mais leve e engraçado.
> Hoje você aprende a **transformar** o mesmo texto para diferentes públicos e formatos — sem precisar reescrever tudo do zero."

---

### [01:00] CONCEITO (2 min)

**[MOSTRE]** Notebook, role até a tabela de conceito.

**[FALE]**
> "Existem 4 tipos de transformação.
>
> **Formato**: mudar como o texto é estruturado. Quest em parágrafo → checklist de missão.
>
> **Tom**: mudar o estilo. Sério → engraçado. Formal → casual.
>
> **Perspectiva**: mudar o ponto de vista. Narrador em 3ª pessoa → personagem em 1ª pessoa.
>
> **Público**: mudar a linguagem para a audiência. Texto técnico para gamer → explicação para quem nunca jogou.
>
> Em todos os casos, o **conteúdo** é o mesmo. O que muda é como ele é apresentado."

---

### [03:00] SETUP (30 seg)

**[EXECUTE]** Setup.

---

### [03:30] DEMONSTRAÇÃO 1 — formato (2 min)

**[MOSTRE]** Primeira demonstração.

**[FALE]**
> "Uma quest escrita em parágrafo sendo transformada em checklist. Vou mostrar o original e depois a transformação."

**[EXECUTE]** Execute.

**[FALE]**
> "O mesmo conteúdo, mas agora em formato de lista que o jogador pode ir marcando."

---

### [05:30] DEMONSTRAÇÃO 2 — tom cômico e post de redes (2 min)

**[MOSTRE]** Segunda demonstração.

**[FALE]**
> "Agora uma cena séria — o dragão Vorathex emergindo das chamas — sendo reescrita de duas formas: cômico e post de redes sociais."

**[EXECUTE]** Execute.

**[FALE]**
> "Olha como o mesmo dragão ficou completamente diferente! O cômico é levinho, e o post de redes sociais ficou perfeito para o Instagram."

---

### [07:30] DEMONSTRAÇÃO 3 — adaptando para públicos (2 min)

**[MOSTRE]** Terceira demonstração.

**[FALE]**
> "Por último: uma descrição técnica de dungeon sendo adaptada para crianças de 8 anos e para quem nunca jogou videogame."

**[EXECUTE]** Execute.

**[FALE]**
> "Perfeito para apresentar o projeto para públicos diferentes — inclusive para o professor que talvez não conheça RPG."

---

### [09:30] SEU TURNO (2 min)

**[MOSTRE]** Célula Seu Turno.

**[FALE]**
> "Peguem qualquer texto do jogo de vocês e transformem para dois públicos ou formatos diferentes.
> Definam o texto nos `???` e as duas transformações. Executem e comparem!"

---

### [11:30] ENCERRAMENTO — na câmera (1 min)

**[CÂMERA]**

**[FALE]**
> "Transformação de texto é muito útil no dia a dia — adaptar e-mails, relatórios, posts, apresentações.
> Na próxima aula, a gente vai usar a IA como crítica — ela vai analisar o texto do nosso mundo e encontrar problemas. Até lá!"

---
---

# 🎬 AULA 12 — Análise Textual: a IA Como Crítica do Seu Mundo
**Arquivo:** `12-analise_textual.ipynb`
**Tempo estimado:** 13 minutos

## ANTES DE GRAVAR
- Abrir o arquivo `12-analise_textual.ipynb` no Jupyter
- Executar o setup antes de gravar
- Conceito central: usar a IA para analisar textos em profundidade — tom, símbolos, consistência

---

### [00:00] ABERTURA — na câmera (1 min)

**[CÂMERA]**

**[FALE]**
> "Aula 12 — penúltima do curso!
> Você criou o lore do seu mundo, mas algo parece errado. As histórias contradizem umas às outras.
> Ou você quer saber se a dungeon realmente parece assustadora do jeito que você escreveu.
> Hoje a IA vira uma **crítica literária** do seu mundo — ela analisa tom, símbolos e inconsistências."

---

### [01:00] CONCEITO (2 min)

**[MOSTRE]** Notebook, role até a tabela.

**[FALE]**
> "Análise textual é pedir para a IA examinar um texto em profundidade.
>
> **Tom e atmosfera**: ela diz se o texto realmente transmite o que você queria. Medo? Maravilha? Alegria?
>
> **Símbolos**: ela identifica o que cada elemento representa além do óbvio. O dragão = corrupção. A chama = esperança.
>
> **Consistência**: ela encontra contradições. 'Aqui você disse que o castelo é impenetrável, mas depois disse que foi invadido há 200 anos.'
>
> Isso é especialmente útil quando seu mundo cresce e fica difícil lembrar de tudo."

---

### [03:00] SETUP (30 seg)

**[EXECUTE]** Setup.

---

### [03:30] DEMONSTRAÇÃO 1 — análise de tom (2 min)

**[MOSTRE]** Primeira demonstração.

**[FALE]**
> "Aqui tem uma descrição de uma sala da dungeon. Vamos pedir para a IA analisar o tom, os recursos literários e o impacto emocional."

**[EXECUTE]** Execute.

**[FALE]**
> "Que análise detalhada! Ela identificou exatamente os recursos — como o 'ar pesado' e as 'tochas tremendo sem motivo' — e explicou por que funcionam para criar tensão."

---

### [05:30] DEMONSTRAÇÃO 2 — análise simbólica (2 min)

**[MOSTRE]** Segunda demonstração.

**[FALE]**
> "Agora a lore da criação do mundo. A IA vai encontrar os símbolos e temas universais escondidos no texto."

**[EXECUTE]** Execute.

**[FALE]**
> "Ela identificou a Chama como símbolo de vida, o Vazio como ignorância ou mal, e os Sombrios como perda de humanidade. São temas que aparecem em mitologias do mundo todo."

---

### [07:30] DEMONSTRAÇÃO 3 — encontrando inconsistências (2 min)

**[MOSTRE]** Terceira demonstração.

**[FALE]**
> "Essa é a minha favorita. Aqui tem um lore com um erro proposital — o reino nunca foi conquistado, mas depois diz que foi ocupado. Vamos ver se a IA pega."

**[EXECUTE]** Execute.

**[FALE]**
> "Pegou! Ela identificou exatamente a contradição. Isso é super útil quando você está construindo um mundo grande e complexo."

---

### [09:30] SEU TURNO (2 min)

**[MOSTRE]** Célula Seu Turno.

**[FALE]**
> "Peguem um trecho do mundo de vocês — lore, cena, descrição — e peçam o tipo de análise que mais interessa: tom, símbolos ou consistência.
> Podem usar qualquer texto que escreveram nas aulas anteriores!"

---

### [11:30] ENCERRAMENTO — na câmera (1 min)

**[CÂMERA]**

**[FALE]**
> "Com análise textual, a IA vira uma parceira de criação — ela aponta o que está funcionando e o que pode melhorar.
> Na próxima e última aula, a gente junta TUDO que aprendeu em um projeto completo. Até lá!"

---
---

# 🎬 AULA 13 — Projeto Final: Construindo o Seu RPG de Texto
**Arquivo:** `13-projeto_final.ipynb`
**Tempo estimado:** 18 minutos

## ANTES DE GRAVAR
- Abrir o arquivo `13-projeto_final.ipynb` no Jupyter
- **Importante:** antes de gravar, preencha as variáveis da Parte 1 com o seu mundo inventado para que o vídeo seja mais dinâmico
- Execute as células 1, 2 e 3 antes de começar para ter os resultados prontos para mostrar

---

### [00:00] ABERTURA — na câmera (2 min)

**[CÂMERA]**

**[FALE]**
> "Chegamos na última aula! O Projeto Final.
>
> Nas 12 aulas anteriores você aprendeu:
> Criar NPCs com personalidade, controlar criatividade, escrever boas instruções, formatar respostas, criar condicionais, ensinar por exemplos, planejar em etapas, raciocinar, resumir, completar, transformar e analisar.
>
> Agora você vai usar **tudo ao mesmo tempo** para construir um RPG de texto completo do zero.
>
> Eu já preenchi o meu — vou mostrar funcionando — mas o mais importante é você criar o seu próprio."

---

### [02:00] PARTE 1 — criando o mundo (2 min)

**[MOSTRE]** Notebook aberto na Parte 1.

**[FALE]**
> "Primeiro passo: definir o mundo. Aqui você preenche 5 variáveis: nome do jogo, gênero, nome do NPC, personalidade e nome do herói.
> Eu já coloquei as minhas — [diga os valores que você preencheu]."

**[EXECUTE]** Execute a célula.

**[FALE]**
> "Pronto! O mundo foi criado. Agora todos os outros trechos vão usar essas variáveis automaticamente."

---

### [04:00] PARTE 2 — a ficha do NPC (2 min)

**[MOSTRE]** Parte 2.

**[FALE]**
> "Aqui usamos o que aprendemos na Aula 01 e 03: o system prompt detalhado com boas práticas.
> O NPC tem regras: fica no personagem, respostas curtas, chama o jogador pelo nome.
> Vou executar e vocês veem o NPC se apresentando."

**[EXECUTE]** Execute.

**[FALE]**
> "Olha ele! Já tem personalidade, já chama o herói pelo nome. Isso é o role system funcionando."

---

### [06:00] PARTE 3 — status do personagem (2 min)

**[MOSTRE]** Parte 3.

**[FALE]**
> "Agora a ficha do herói usando output estruturado — da Aula 04. O system tem o template da ficha e a IA preenche para o nosso personagem."

**[EXECUTE]** Execute.

**[FALE]**
> "Ficha gerada! Com classe, HP, habilidade especial, inventário e missão atual. Pronto para o jogo."

---

### [08:00] PARTE 4 — a missão com escolhas (3 min)

**[MOSTRE]** Parte 4.

**[FALE]**
> "Aqui combinamos Aula 05 (condicionais) e Aula 06 (few-shot). O NPC apresenta a missão e reage diferente dependendo da escolha do jogador.
> Primeiro vou executar a apresentação da missão..."

**[EXECUTE]** Execute a primeira célula da Parte 4.

**[FALE]**
> "Agora vou escolher como o herói vai reagir. Eu coloquei [diga sua escolha]..."

**[EXECUTE]** Execute a segunda célula.

**[FALE]**
> "O NPC reagiu exatamente de acordo com o tipo de escolha! Isso é few-shot e condicional trabalhando juntos."

---

### [11:00] PARTE 5 — o chefe final (3 min)

**[MOSTRE]** Parte 5.

**[FALE]**
> "Toda boa história tem um chefe final. Aqui o NPC usa Chain of Thought — da Aula 08 — para analisar o inimigo e criar um plano estratégico.
> Eu coloquei o [nome do chefe que você definiu]."

**[EXECUTE]** Execute.

**[FALE]**
> "O raciocínio ficou explícito — analisou pontos fracos, calculou riscos e propôs um plano de 3 movimentos. Exatamente o que um bom conselheiro faria."

---

### [14:00] PARTE 6 — modo livre (2 min)

**[MOSTRE]** Parte 6.

**[FALE]**
> "A Parte 6 é o modo livre — vocês continuam a história como quiserem.
> Aqui não tem resposta certa. Experimentem mudar a temperature, adicionar contexto, criar novos personagens.
> O jogo é de vocês."

**[EXECUTE]** Execute a célula com uma cena de sua escolha.

---

### [16:00] ENCERRAMENTO FINAL — na câmera (2 min)

**[CÂMERA]** Apareça com energia.

**[FALE]**
> "E esse é o poder da Engenharia de Prompt.
>
> Com o que vocês aprenderam neste curso, vocês conseguem criar NPCs com personalidade, construir mundos completos, fazer a IA raciocinar, adaptar conteúdo para qualquer público...
>
> Mas mais do que isso: agora vocês sabem **como se comunicar com qualquer IA** de forma clara, precisa e criativa. Isso vai ser útil em qualquer área — escola, trabalho, projetos pessoais.
>
> O código de vocês está no Moodle para baixar. O desafio final é: completem o notebook do Projeto Final com o **mundo de vocês**.
>
> Obrigado por assistir! Até o próximo projeto."
