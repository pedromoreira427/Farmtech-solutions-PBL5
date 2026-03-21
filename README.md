# FIAP - Faculdade de Informática e Administração Paulista

## FarmTech Solutions — Previsão de Rendimento de Safra

## Grupo FarmTech

###  Integrantes:
* **Pedro Gustavo Franca Moreira**
* **RM568262**

###  Professores:

**Coordenador(a)**
* *(André Godoi)*

---

## 📜 Descrição
**Entrega 1 — Machine Learning:**

O objetivo desta entrega é analisar uma base de dados com informações de condições climáticas e de solo — precipitação, umidade específica, umidade relativa e temperatura — relacionadas ao rendimento de quatro culturas agrícolas: Cocoa beans, Oil palm fruit, Rice paddy e Rubber natural.

A partir desses dados, foram realizadas três etapas principais. Primeiro, uma análise exploratória completa do dataset, com estatísticas descritivas, visualização de distribuições, análise de correlação entre variáveis e comparação de rendimento por cultura. Segundo, uma clusterização utilizando o algoritmo K-Means para identificar tendências e grupos naturais nos dados, com aplicação do método Elbow para definição do número ideal de clusters, visualização via PCA e detecção de outliers pelo método IQR. Terceiro, o desenvolvimento de cinco modelos preditivos de regressão supervisionada — Regressão Linear, Árvore de Decisão, Random Forest, Gradient Boosting e K-Nearest Neighbors — avaliados com as métricas MAE, RMSE e R², além de validação cruzada 5-fold para garantir a generalização dos modelos.

**Entrega 2 — Computação em Nuvem (AWS):**

Para hospedar a API que recebe os dados dos sensores de campo e executa o modelo de Machine Learning, foi realizada uma estimativa de custos utilizando a AWS Pricing Calculator, comparando as regiões de São Paulo (BR) e Virgínia do Norte (EUA) para uma instância EC2 t3.micro Linux com 2 vCPUs, 1 GiB de memória, rede de até 5 Gigabit e 50 GB de armazenamento HDD, no modelo de pagamento On-Demand.

A região de Virgínia do Norte apresentou custo mensal de $3,80 USD, enquanto São Paulo apresentou $6,13 USD — uma diferença de aproximadamente 38%. No entanto, considerando as restrições legais impostas pela LGPD (Lei nº 13.709/2018) sobre armazenamento de dados no exterior e a necessidade de baixa latência para acesso em tempo real aos dados dos sensores instalados na fazenda, a região de **São Paulo** foi escolhida como a solução mais adequada para este projeto.

---

## 📁 Estrutura de pastas

Dentre os arquivos e pastas presentes na raiz do projeto, definem-se:

- **.github**: arquivos de configuração específicos do GitHub para gerenciamento e automação de processos no repositório.
- **assets**: arquivos relacionados a elementos não-estruturados do repositório, como imagens e capturas de tela da calculadora AWS.
- **config**: arquivos de configuração com parâmetros e ajustes do projeto.
- **document**: documentos do projeto solicitados pelas atividades. Na subpasta "other", documentos complementares.
- **scripts**: scripts auxiliares para tarefas específicas do projeto.
- **src**: código fonte desenvolvido ao longo das fases, incluindo o notebook Jupyter principal.
- **README.md**: arquivo que serve como guia e explicação geral sobre o projeto.

---

## 🔧 Como executar o código

### Pré-requisitos

- Conta Google (para acesso ao Google Colab)
- Arquivo `crop_yield.csv` disponível localmente

### Passo a passo

**Fase 1 — Acessar o notebook:**

1. Acesse o arquivo `pedrogustavofrancamoreira_rm568262_pbl_fase5.ipynb` na pasta `src/` deste repositório
2. Clique em **"Open in Colab"** ou acesse o Google Colab em https://colab.research.google.com e faça o upload do notebook

**Fase 2 — Carregar o dataset:**

1. Execute a célula da Seção 1 (Importação de Bibliotecas)
2. Execute a célula de carregamento da Seção 2 — um seletor de arquivo será aberto
3. Selecione o arquivo `crop_yield.csv` disponível neste repositório

**Fase 3 — Executar o notebook:**

1. Execute as células na ordem apresentada (Seção 1 → Seção 2 → ... → Seção 5)
2. Os gráficos e resultados serão exibidos inline ao longo do notebook

### Bibliotecas utilizadas

- `pandas` — manipulação de dados
- `numpy` — operações numéricas
- `matplotlib` / `seaborn` — visualização de dados
- `scikit-learn` — modelos de Machine Learning e pré-processamento


---

## 🗃 Histórico de lançamentos

* 0.1.0 - *(20/03/26)* — Versão inicial: análise exploratória e clusterização
* 0.2.0 - *(20/03/26)* — Adição dos 5 modelos preditivos de regressão
* 0.3.0 - *(20/03/26)* — Estimativa de custos AWS e justificativa de região
* 0.4.0 - *(21/03/26)* — Revisão geral e documentação final
* 0.5.0 - *(21/03/26)* — Entrega final

---

## 📹 Vídeos Demonstrativos

- **Entrega 1 — Machine Learning:** *(https://youtu.be/b3dY15Qy7i0?si=0UMVP6yN9I73wLca)*
- **Entrega 2 — AWS Cloud:** *(https://youtu.be/YU79-mJUoQU?si=t56HNyUZOsZRlr9x)*
