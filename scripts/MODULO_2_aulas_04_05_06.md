# 🎮 MÓDULO 2 — Scripts das Aulas 04, 05 e 06
**Integrante responsável:** ________________________________
**Tema do módulo:** Estrutura — formatos de resposta e lógica condicional

> 📌 **Como usar este script:**
> - Abra o notebook da aula no Jupyter antes de começar
> - Leia tudo com calma uma vez antes de gravar
> - **[FALE]** = diga isso | **[EXECUTE]** = clique no botão ▶ da célula | **[MOSTRE]** = role até esta parte

---

---

# 🎬 AULA 04 — Output Estruturado: Fichas, Cards e Inventários
**Arquivo:** `04-output_estruturado.ipynb`
**Tempo estimado:** 14 minutos

## ANTES DE GRAVAR
- Abrir o arquivo `04-output_estruturado.ipynb` no Jupyter
- Executar a célula de setup e confirmar que não deu erro
- Esta aula tem 4 demonstrações — leia todas antes de gravar

---

### [00:00] ABERTURA — na câmera (1 min)

**[CÂMERA]** Apareça sorrindo.

**[FALE]**
> "Olá! Sou [seu nome] e estou assumindo o Módulo 2 do nosso curso.
> Nas aulas anteriores, você aprendeu a criar NPCs e dar boas instruções para a IA.
> Mas agora surge um problema: você precisa mostrar a ficha do personagem na tela do jogo, mas a IA sempre devolve um parágrafo bagunçado.
> Hoje você aprende a **controlar exatamente como a resposta vai aparecer** — tabelas, listas, cards, JSON. Tudo organizado."

---

### [01:00] CONCEITO (2 min)

**[MOSTRE]** Notebook aberto, role até o conceito.

**[FALE]**
> "O segredo é simples: você passa o **molde** para a IA no system prompt.
>
> É como dar ao escriba do reino um formulário. Sem formulário, ele escreve um rolo de pergaminho confuso.
> Com o formulário preenchido de campos, ele coloca cada informação no lugar certo.
>
> Você vai ver a IA gerando tabelas de atributos, cards de item mágico, listas de habilidades e até dados em JSON — que é o formato que os programas usam para guardar informações."

---

### [03:00] SETUP (30 seg)

**[EXECUTE]** Execute o setup.

**[FALE]** "Conectado. Vamos lá."

---

### [03:30] DEMONSTRAÇÃO 1 — ficha de personagem em tabela (2 min)

**[MOSTRE]** Primeira demonstração.

**[FALE]**
> "A primeira demo gera uma ficha de personagem em formato de tabela. O system prompt tem o molde da tabela — com os campos Nome, Classe, Nível, HP e atributos.
> A IA vai preencher esses campos para o personagem que a gente pedir."

**[EXECUTE]** Execute.

**[FALE]**
> "Olha que organizado! Uma tabela completa, pronta para usar no jogo. E o segredo foi passar o template da tabela no system."

---

### [05:30] DEMONSTRAÇÃO 2 — card de item mágico (2 min)

**[MOSTRE]** Segunda demonstração.

**[FALE]**
> "Agora um card de item. Olhem o format no system: emoji, nome, tipo, poder, maldição e valor.
> A IA vai gerar um card seguindo exatamente esse molde para qualquer item que a gente pedir."

**[EXECUTE]** Execute.

**[FALE]**
> "Perfeito né? Um card limpo e consistente. Todo item do jogo vai ter o mesmo formato — porque a gente definiu o template uma vez e a IA segue."

---

### [07:30] DEMONSTRAÇÃO 3 — log em JSON (2 min)

**[MOSTRE]** Terceira demonstração.

**[FALE]**
> "Essa é para quem vai programar um jogo de verdade. JSON é o formato que programas usam para guardar dados.
> Aqui a gente pede o log da missão em JSON — com campos específicos que qualquer código consegue ler."

**[EXECUTE]** Execute.

**[FALE]**
> "Viram? A IA retornou um JSON estruturado. Se você quiser usar isso num app ou site, já está no formato certo."

---

### [09:30] DEMONSTRAÇÃO 4 — checklist (1 min)

**[MOSTRE]** Quarta demonstração.

**[FALE]**
> "Por último: um checklist. Simples, mas super útil para listas de preparação antes de uma dungeon."

**[EXECUTE]** Execute.

---

### [10:30] SEU TURNO (2 min)

**[MOSTRE]** Célula Seu Turno.

**[FALE]**
> "Agora é com vocês! Criem o card de um item mágico inventado por vocês mesmos.
> Mudem o system para o formato que quiserem — adicionem ou removam campos.
> Substituam os `???` e executem!"

---

### [12:30] ENCERRAMENTO — na câmera (1 min)

**[CÂMERA]**

**[FALE]**
> "Agora você sabe fazer a IA entregar dados organizados em qualquer formato.
> Na próxima aula, a gente vai ver algo bem legal: como fazer o NPC mudar de comportamento dependendo de quem está falando com ele. Até lá!"

---
---

# 🎬 AULA 05 — Condicionais: NPCs que Reagem ao Contexto
**Arquivo:** `05-condicoes.ipynb`
**Tempo estimado:** 13 minutos

## ANTES DE GRAVAR
- Abrir o arquivo `05-condicoes.ipynb` no Jupyter
- Executar o setup antes de gravar
- Conceito central: SE...ENTÃO no prompt = comportamento do NPC baseado em contexto

---

### [00:00] ABERTURA — na câmera (1 min)

**[CÂMERA]**

**[FALE]**
> "Aula 05! Você já sabe criar NPCs com formato e personalidade.
> Mas imagina: o guarda da cidade deveria ser super respeitoso com um herói famoso e super desconfiado com um ladrão.
> O mesmo NPC, comportamentos completamente diferentes.
> Hoje você aprende a fazer isso com **condicionais no prompt** — regras do tipo 'SE isso, ENTÃO aquilo'."

---

### [01:00] CONCEITO (2 min)

**[MOSTRE]** Notebook, role até o conceito.

**[FALE]**
> "Condicionais no prompt são como as **regras de comportamento do NPC** no manual do mestre.
>
> Você escreve no system: 'SE o jogador é guerreiro, seja respeitoso. SE o jogador é ladrão, desconfie.'
>
> A IA lê essas regras e as aplica automaticamente dependendo do que o usuário escrever.
>
> E existe também o **fallback** — que é o que o NPC faz quando a situação não se encaixa em nenhuma regra. Tipo o NPC dizer 'não entendi, pode explicar melhor?'"

---

### [03:00] SETUP (30 seg)

**[EXECUTE]** Setup.

---

### [03:30] DEMONSTRAÇÃO 1 — guarda que reage pela classe (3 min)

**[MOSTRE]** Primeira demonstração.

**[FALE]**
> "Aqui o Guarda Torvin tem regras para cada classe. Guerreiro, Mago, Ladino — cada um recebe um tratamento diferente.
> Vou rodar para os três e vocês vejam ao vivo."

**[EXECUTE]** Execute.

**[FALE]** Enquanto os resultados aparecem:
> "Olha como ele mudou! Com o guerreiro foi respeitoso. Com o mago, cauteloso. Com o ladino, já botou a mão na espada.
> Mesmo NPC, mesma pergunta, comportamentos completamente diferentes — só porque a classe mudou."

---

### [06:30] DEMONSTRAÇÃO 2 — reputação (2 min)

**[MOSTRE]** Segunda demonstração.

**[FALE]**
> "Agora a estalajadeira Marta reage pela reputação do jogador — herói lendário, aventureiro normal ou criminoso procurado. Mesmo princípio."

**[EXECUTE]** Execute.

**[FALE]**
> "Perfeito! Um sistema de reputação funcional criado só com texto no prompt."

---

### [08:30] DEMONSTRAÇÃO 3 — fallback (1 min)

**[MOSTRE]** Terceira demonstração.

**[FALE]**
> "E o fallback — o que acontece quando o jogador pergunta algo fora do script.
> O Oráculo não responde perguntas de culinária, então veja o que acontece."

**[EXECUTE]** Execute.

**[FALE]**
> "Ele redirecionou! Disse que está além da visão dele e sugeriu perguntas que ele pode responder. Isso mantém o NPC no personagem."

---

### [09:30] SEU TURNO (2 min)

**[MOSTRE]** Célula Seu Turno.

**[FALE]**
> "Agora criem o NPC de vocês com pelo menos 3 condições. Pensem: quando o jogador diz X, o NPC faz Y. Quando diz W, faz Z. E o fallback: o que ele faz quando não entende."

---

### [11:30] ENCERRAMENTO — na câmera (1 min)

**[CÂMERA]**

**[FALE]**
> "Condicionais são poderosas porque deixam o NPC parecer inteligente e dinâmico.
> Na próxima aula, você vai aprender a ensinar a IA por exemplos — sem precisar descrever todas as regras. Se chama few-shot e é muito elegante. Até lá!"

---
---

# 🎬 AULA 06 — Few-Shot: Ensinando o NPC pelo Exemplo
**Arquivo:** `06-few_shot.ipynb`
**Tempo estimado:** 13 minutos

## ANTES DE GRAVAR
- Abrir o arquivo `06-few_shot.ipynb` no Jupyter
- Executar o setup antes de gravar
- Conceito central: mostrar exemplos de diálogo ao NPC em vez de descrever regras

---

### [00:00] ABERTURA — na câmera (1 min)

**[CÂMERA]**

**[FALE]**
> "Aula 06 — a minha favorita!
> Você quer que o ferreiro do jogo fale como um velho rabugento com sotaque diferente.
> Você poderia escrever 20 regras no system prompt descrevendo como ele fala...
> Ou você poderia simplesmente **mostrar 3 exemplos** e a IA vai captar o estilo automaticamente.
> Isso é o few-shot. E é muito mais eficiente."

---

### [01:00] CONCEITO (2 min)

**[MOSTRE]** Notebook, role até a tabela de conceito.

**[FALE]**
> "Existem três variações.
>
> **Zero-shot**: nenhum exemplo. Você só descreve quem é o personagem. A IA tenta, mas muitas vezes fica genérica.
>
> **One-shot**: um exemplo. Você mostra um diálogo de referência. Já melhora bastante.
>
> **Few-shot**: vários exemplos — geralmente 3 a 5. Você mostra o personagem em ação várias vezes e a IA aprende o estilo.
>
> É como dar ao ator um roteiro de ensaio antes de ele entrar em cena."

---

### [03:00] SETUP (30 seg)

**[EXECUTE]** Setup.

---

### [03:30] DEMONSTRAÇÃO — zero, one e few-shot lado a lado (6 min)

**[MOSTRE]** A demonstração principal.

**[FALE]**
> "Aqui a gente vai ver o mesmo ferreiro — o Brun — com zero, one e few-shot para a mesma pergunta.
> Vou executar e a gente compara ao vivo."

**[EXECUTE]** Execute toda a célula.

**[FALE]** Enquanto os resultados aparecem:
> "Com zero-shot: respondeu, mas qualquer ferreiro de qualquer jogo poderia ter dito isso. Sem personalidade única.
>
> Com one-shot: já ficou mais interessante — deu pra perceber alguma diferença no jeito de falar.
>
> Com few-shot: olha só! Ele falou com sotaque nordestino, com expressões únicas, orgulho do trabalho...
> Isso é consistente. Toda vez que o jogador falar com o Brun, vai reconhecer o personagem.
>
> O segredo é: os exemplos que você passa no `assistant` dentro do few-shot ensinam o estilo muito melhor do que qualquer descrição textual."

---

### [09:30] SEU TURNO (2 min)

**[MOSTRE]** Célula Seu Turno.

**[FALE]**
> "Agora criem o NPC de vocês com pelo menos 3 exemplos de diálogo.
> Inventem um personagem — pode ser uma bruxa, um rei, um fantasma — e mostrem como ele fala em 3 situações diferentes.
> A IA vai captar o estilo e responder na 4ª pergunta no mesmo tom."

---

### [11:30] ENCERRAMENTO — na câmera (1 min)

**[CÂMERA]**

**[FALE]**
> "Few-shot é uma das técnicas mais poderosas da engenharia de prompt. Com poucos exemplos, você consegue resultados que 100 linhas de instrução não conseguiriam.
> O Módulo 3 começa agora com [nome do Integrante C], que vai mostrar como criar dungeons em múltiplos passos e fazer a IA raciocinar. Até lá!"
