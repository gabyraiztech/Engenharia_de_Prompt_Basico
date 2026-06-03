# 🎮 Engenharia de Prompt — Construindo um RPG com IA

> Curso introdutório de Engenharia de Prompt para o Ensino Médio.
> Aprenda a conversar com Inteligências Artificiais enquanto constrói o seu próprio jogo de RPG de texto.

---

## 📖 Sobre o curso

Este curso ensina os principais conceitos de **Engenharia de Prompt** de forma prática e divertida.
Cada aula usa um único tema — a construção de um RPG de texto — para que o aluno veja como cada técnica se encaixa em um projeto real.

Ao final do curso, o aluno terá criado um chatbot interativo com personagens, missões, chefe final e narrativa própria.

**Tecnologia utilizada:** Python + Groq API + Jupyter Notebook
**Nível:** Iniciante — sem experiência prévia em programação necessária
**Público:** Ensino Médio

---

## 🗺️ Estrutura do Curso

### Módulo 1 — Fundamentos
| Aula | Tema | O que você aprende |
|------|------|-------------------|
| 01 | Roles | Como definir a personalidade de um NPC com `system`, `user` e `assistant` |
| 02 | Parâmetros | Controlar criatividade com `temperature` e `top_p` |
| 03 | Boas Práticas | Escrever prompts claros e específicos |

### Módulo 2 — Estrutura
| Aula | Tema | O que você aprende |
|------|------|-------------------|
| 04 | Output Estruturado | Gerar fichas, cards, listas e JSON |
| 05 | Condicionais | NPCs que reagem diferente conforme o contexto |
| 06 | Few-Shot | Ensinar a IA por exemplos de diálogo |

### Módulo 3 — Técnicas
| Aula | Tema | O que você aprende |
|------|------|-------------------|
| 07 | Multi-Step | Construir dungeons passo a passo |
| 08 | Chain of Thought | Fazer a IA raciocinar em voz alta |
| 09 | Sumarização | Resumir logs de aventura em diferentes estilos |

### Módulo 4 — Aplicações
| Aula | Tema | O que você aprende |
|------|------|-------------------|
| 10 | Complemento de Texto | Continuar lendas e expandir lore |
| 11 | Transformação de Texto | Adaptar o jogo para públicos diferentes |
| 12 | Análise Textual | Usar a IA para revisar e analisar narrativas |
| 13 | 🏆 Projeto Final | Construir o RPG completo com tudo que aprendeu |

---

## ⚙️ Como configurar o ambiente

### 1. Pré-requisitos
- Python 3.10 ou superior
- Jupyter Notebook ou VS Code com extensão Jupyter

### 2. Instalar as dependências

```bash
pip install groq python-dotenv
```

### 3. Criar a chave de API

1. Acesse [console.groq.com](https://console.groq.com) e crie uma conta gratuita
2. Gere uma API Key
3. Crie um arquivo `.env` na raiz do projeto com o conteúdo:

```
GROQ_API=sua_chave_aqui
```

> ⚠️ **Nunca compartilhe sua chave de API.** O arquivo `.env` não é enviado ao GitHub.

### 4. Rodar o primeiro notebook

Abra o arquivo `01-roles.ipynb` no Jupyter e execute a célula de setup. Se não aparecer erro, está tudo pronto!

---

## 📁 Estrutura dos arquivos

```
engenharia_prompt/
│
├── 00-template_estrutura.ipynb   # Molde padrão de aula (referência)
├── 01-roles.ipynb
├── 02-params.ipynb
├── 03-boas_praticas.ipynb
├── 04-output_estruturado.ipynb
├── 05-condicoes.ipynb
├── 06-few_shot.ipynb
├── 07-steps.ipynb
├── 08-cot.ipynb
├── 09-sumarizacao.ipynb
├── 10-texto_complemento.ipynb
├── 11-transformacao_texto.ipynb
├── 12-analise_textual.ipynb
├── 13-projeto_final.ipynb        # Projeto capstone
│
├── scripts/                      # Materiais para gravação das aulas
│   ├── 00_DIVISAO_E_MOODLE.md    # Divisão do grupo + guia do Moodle
│   ├── MODULO_1_aulas_01_02_03.md
│   ├── MODULO_2_aulas_04_05_06.md
│   ├── MODULO_3_aulas_07_08_09.md
│   └── MODULO_4_aulas_10_11_12_projeto.md
│
└── .env                          # Sua chave de API (não versionado)
```

---

## 🛠️ Tecnologias

| Tecnologia | Uso |
|---|---|
| [Python](https://python.org) | Linguagem de programação |
| [Jupyter Notebook](https://jupyter.org) | Ambiente interativo de aprendizado |
| [Groq API](https://groq.com) | Acesso ao modelo de linguagem (LLM) |
| [LLaMA 3.3 70B](https://groq.com) | Modelo de IA utilizado nas aulas |
| [python-dotenv](https://pypi.org/project/python-dotenv/) | Gerenciamento seguro da API Key |

---

## 👥 Equipe

Projeto desenvolvido para a disciplina de **Tecnologias Digitais para o Ensino (TDE)**.

| Integrante | Módulo |
|---|---|
| [nome] | Módulo 1 — Aulas 01, 02, 03 |
| [nome] | Módulo 2 — Aulas 04, 05, 06 |
| [nome] | Módulo 3 — Aulas 07, 08, 09 |
| [nome] | Módulo 4 — Aulas 10, 11, 12, 13 |

---

## 📄 Licença

Este projeto é de uso educacional livre.
Sinta-se à vontade para usar, adaptar e compartilhar com sua turma.
