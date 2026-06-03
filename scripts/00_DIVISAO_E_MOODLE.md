# 📚 Curso: Engenharia de Prompt — Organização do Grupo e Estrutura no Moodle

---

## 👥 Divisão entre os 4 integrantes

> Cada pessoa é responsável por **gravar os vídeos, apresentar os conceitos e conduzir os exercícios** das aulas do seu módulo.
> Os scripts com o que falar estão nos arquivos `MODULO_1`, `MODULO_2`, `MODULO_3` e `MODULO_4`.

| Módulo | Integrante | Aulas | Tema geral |
|--------|-----------|-------|------------|
| **Módulo 1** | Integrante A *(quem conhece o conteúdo)* | 01, 02, 03 | Fundamentos — como a IA funciona e como dar ordens a ela |
| **Módulo 2** | Integrante B | 04, 05, 06 | Estrutura — formatos de resposta e lógica condicional |
| **Módulo 3** | Integrante C | 07, 08, 09 | Técnicas — planejamento em etapas e raciocínio da IA |
| **Módulo 4** | Integrante D | 10, 11, 12, 13 | Aplicações — texto, narrativa e projeto final |

---

## ⏱️ Tempo estimado por aula

| Tipo de célula | Tempo na gravação |
|---|---|
| Abertura + MISSÃO DO DIA | 1 min |
| Explicação do conceito | 2-3 min |
| Demonstrações de código | 5-7 min |
| "Seu Turno" | 2 min |
| Glossário + encerramento | 1 min |
| **Total por aula** | **~12-15 min** |

---

## 🎬 Como gravar os vídeos

### O que você vai precisar
- Computador com Jupyter Notebook aberto
- Software de gravação de tela (OBS, Loom, Gravador do Windows ou Google Meet)
- Microfone ou fone com microfone
- Script da sua aula aberto em outra janela (leia enquanto grava)

### Formato do vídeo
1. Apareça na câmera por 15 segundos na abertura e fechamento
2. O resto do tempo: **tela compartilhada com o notebook**
3. Execute as células em tempo real — não precisa editar o vídeo

### Dica importante
> Leia o script antes de gravar pelo menos uma vez. Teste executar todas as células para garantir que funcionam. Se uma célula der erro, não entre em pânico — diga "vamos ajustar isso" e corrija ao vivo.

---

## 🖥️ Como organizar no Moodle

O Moodle é uma plataforma de ensino onde você sobe os materiais e os alunos acessam. Veja como estruturar:

### Estrutura sugerida no Moodle

```
📁 CURSO: Engenharia de Prompt — Construindo um RPG com IA
│
├── 📌 Apresentação do curso (texto + vídeo de boas-vindas)
│
├── 📦 MÓDULO 1 — Fundamentos (Integrante A)
│   ├── 🎬 Vídeo: Aula 01 — Roles
│   ├── 📄 Arquivo: 01-roles.ipynb (para download)
│   ├── 🎬 Vídeo: Aula 02 — Parâmetros
│   ├── 📄 Arquivo: 02-params.ipynb
│   ├── 🎬 Vídeo: Aula 03 — Boas Práticas
│   ├── 📄 Arquivo: 03-boas_praticas.ipynb
│   └── 📝 Atividade: "Crie seu primeiro NPC" (fórum ou envio de arquivo)
│
├── 📦 MÓDULO 2 — Estrutura (Integrante B)
│   ├── 🎬 Vídeo: Aula 04 — Output Estruturado
│   ├── 📄 Arquivo: 04-output_estruturado.ipynb
│   ├── 🎬 Vídeo: Aula 05 — Condicionais
│   ├── 📄 Arquivo: 05-condicoes.ipynb
│   ├── 🎬 Vídeo: Aula 06 — Few-Shot
│   ├── 📄 Arquivo: 06-few_shot.ipynb
│   └── 📝 Atividade: "Crie um NPC com personalidade única"
│
├── 📦 MÓDULO 3 — Técnicas (Integrante C)
│   ├── 🎬 Vídeo: Aula 07 — Multi-Step
│   ├── 📄 Arquivo: 07-steps.ipynb
│   ├── 🎬 Vídeo: Aula 08 — Chain of Thought
│   ├── 📄 Arquivo: 08-cot.ipynb
│   ├── 🎬 Vídeo: Aula 09 — Sumarização
│   ├── 📄 Arquivo: 09-sumarizacao.ipynb
│   └── 📝 Atividade: "Crie e resolva um enigma de dungeon"
│
└── 📦 MÓDULO 4 — Aplicações + Projeto (Integrante D)
    ├── 🎬 Vídeo: Aula 10 — Complemento de Texto
    ├── 📄 Arquivo: 10-texto_complemento.ipynb
    ├── 🎬 Vídeo: Aula 11 — Transformação de Texto
    ├── 📄 Arquivo: 11-transformacao_texto.ipynb
    ├── 🎬 Vídeo: Aula 12 — Análise Textual
    ├── 📄 Arquivo: 12-analise_textual.ipynb
    ├── 🎬 Vídeo: Aula 13 — Projeto Final
    ├── 📄 Arquivo: 13-projeto_final.ipynb
    └── 📝 Atividade FINAL: "Publique seu RPG de texto" (envio do notebook completo)
```

### Passo a passo para adicionar um vídeo no Moodle
1. Entre no curso no Moodle como professor/editor
2. Clique em **"Ativar edição"** (botão no canto superior direito)
3. Dentro do módulo correto, clique em **"Adicionar uma atividade ou recurso"**
4. Escolha **"Arquivo"** para subir o notebook (.ipynb) ou **"URL"** se o vídeo estiver no YouTube/Drive
5. Para vídeos grandes: suba no **Google Drive** ou **YouTube (não listado)** e cole o link no Moodle
6. Para atividades: escolha **"Tarefa"** (envio de arquivo) ou **"Fórum"** (discussão)

---

## ✅ Checklist antes de publicar no Moodle

- [ ] Todos os vídeos gravados e revisados
- [ ] Notebooks testados (todas as células funcionam com a API key)
- [ ] Estrutura do Moodle criada com os 4 módulos
- [ ] Vídeos subidos no Drive/YouTube e links copiados
- [ ] Notebooks subidos como arquivos para download
- [ ] Pelo menos 1 atividade por módulo criada
- [ ] Apresentação do curso escrita (o que o aluno vai aprender)
