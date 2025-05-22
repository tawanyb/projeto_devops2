
# 🤖 Desafio Técnico: Agente de IA para Rateio de Custos com CrewAI

Este projeto implementa um **Agente de IA com CrewAI** capaz de ler planilhas, calcular rateio de custos entre colaboradores, e gerar insights visuais de forma automatizada, utilizando agentes autônomos com o poder da LLM da Groq.

---

## 📌 Objetivo

Criar uma solução em Python e Google Colab, utilizando a biblioteca [CrewAI](https://github.com/joaomdmoura/crewai), para:

- 📥 Ler planilhas de colaboradores, ferramentas e benefícios
- 📊 Consolidar os dados por colaborador
- 🧮 Calcular o rateio de custos com base nas regras do desafio
- 📈 Gerar gráficos e insights visuais
- 📤 Exportar os resultados para a pasta `/output`

---

## 📁 Estrutura de Diretórios

```
.
├── data/
│   ├── Dados Colaboradores.xlsx
│   ├── beneficios/
│   │   ├── Beneficio 1 - Unimed.xlsx
│   │   └── Beneficio 2 - Gympass.xlsx
│   └── ferramentas/
│       ├── Ferramenta 1 - Github.xlsx
│       └── Ferramenta 2 - Google workspace.xlsx
│
├── output/
│   ├── dados_consolidados.xlsx
│   ├── relatorio_rateio.xlsx
│   └── grafico_rateio.png
│
├── notebook/
│   └── desafio_rateio_agente_ia.ipynb
│
├── README.md
```

---

## 🚀 Execução no Google Colab

1. **Abra o notebook Colab**:
   - [🔗 Acesse aqui o notebook](https://colab.research.google.com/)

2. **Suba os arquivos na estrutura abaixo**:

```
/content/data/
├── Dados Colaboradores.xlsx
├── beneficios/
│   ├── Beneficio 1 - Unimed.xlsx
│   └── Beneficio 2 - Gympass.xlsx
└── ferramentas/
    ├── Ferramenta 1 - Github.xlsx
    └── Ferramenta 2 - Google workspace.xlsx
```

3. **Configure a chave da API da Groq** no Colab:

```python
from google.colab import userdata
userdata.set('chaviapigroq', 'SUA_API_KEY')
```

4. **Execute o notebook completo** e os resultados aparecerão em `/content/output/`.

---

## 🧠 Desenvolvimento e Fontes de Estudo

Durante o desenvolvimento, foram utilizadas as seguintes fontes de aprendizado:

### 📺 YouTube – Aprendendo CrewAI

- [CrewAI: Agentes Autônomos com Python (por LablabAI)](https://www.youtube.com/watch?v=dpQ9HznPDCk)
- [Como usar CrewAI com LangChain (João Moura - Criador)](https://www.youtube.com/watch?v=nHeS92ABq9c)
- [CrewAI Tools explicadas (Oficial)](https://www.youtube.com/watch?v=rYO9pZAv5ow)

### 📚 Documentação Oficial

- [CrewAI GitHub](https://github.com/joaomdmoura/crewai)
- [CrewAI Tools](https://github.com/joaomdmoura/crewai-tools)
- [Groq API para LLM](https://console.groq.com/keys)

---

## 🤖 Agentes Utilizados

| Agente                  | Função                                                                 |
|-------------------------|------------------------------------------------------------------------|
| `leitor_agent`          | Lê e padroniza todas as planilhas                                      |
| `processador_agent`     | Calcula o rateio com base nas regras definidas                         |
| `gerador_de_visual_agent` | Gera visualizações (gráficos e insights de negócio)                    |

---

## 📦 Saída Esperada

| Arquivo                      | Descrição                                                    |
|-----------------------------|---------------------------------------------------------------|
| `dados_consolidados.xlsx`   | Planilha com os dados lidos e padronizados                   |
| `relatorio_rateio.xlsx`     | Custos por colaborador (benefícios + ferramentas)            |
| `grafico_rateio.png`        | Gráfico com visão geral dos custos                           |

---

## 🛠️ Tecnologias Utilizadas

- Python 3.10+
- [Google Colab](https://colab.research.google.com/)
- [CrewAI](https://github.com/joaomdmoura/crewai)
- [CrewAI Tools](https://github.com/joaomdmoura/crewai-tools)
- [Groq LLM](https://console.groq.com/)
- Pandas, Matplotlib, OpenPyXL

---

## 📄 Licença

Este projeto é livre para fins educacionais, técnicos e de demonstração de IA aplicada com agentes.  
Desenvolvido como parte de um **desafio técnico de IA com foco em CrewAI**.
