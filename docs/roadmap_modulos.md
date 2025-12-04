# Roadmap dos Módulos – Curso pessoal de Ciência de Dados (FinTrack)

Este documento descreve como cada módulo de estudo contribui para a evolução do FinTrack.

## Módulo 0 – Kit de Ferramentas & Setup do FinTrack

### Objetivos principais

Escolher e dominar ferramentas básicas:

- VS Code como IDE principal.

- Jupyter para exploração de dados.

- Criar o projeto FinTrack com estrutura organizada.

- Criar e ativar ambiente virtual (venv).

- Inicializar repositório Git e conectar ao GitHub.

- Escrever README inicial e este roadmap.

- Entregáveis

    - Pasta fintrack/ com venv, estrutura de pacotes e script fintrack/main.py.

    - Repositório Git conectado ao GitHub (riomarfilho/fintrack).

    - README.md com visão geral do projeto e instruções de execução.

    - docs/roadmap_modulos.md com o planejamento dos próximos módulos.

## Módulo 1 – Fundamentos de Python para Dados

### Foco de estudo

Sintaxe essencial de Python usada em projetos de dados:

- tipos básicos, coleções, funções, módulos.

- Boas práticas iniciais (nomes de variáveis, organização de arquivos).

- Leitura e escrita de arquivos (CSV, JSON simples).

- Impacto no FinTrack

- Criar funções simples para:

    - ler arquivos de operações em formato CSV/planilha exportada;

    - validar estrutura básica dos dados (colunas obrigatórias, tipos etc.).

    - Iniciar uma área fintrack/io/ para lidar com entrada de dados.

## Módulo 2 – Pandas e Manipulação de Dados Financeiros

Foco de estudo

Introdução estruturada ao pandas:

DataFrame, Series, indexação, filtragem.

agregações, groupby, merges/joins.

Trabalho com datas e números financeiros.

Impacto no FinTrack

Implementar carregamento das operações em pandas.

Padronizar o formato interno das operações (compra, venda, quantidade, preço, taxas).

Calcular:

posição atual por ativo;

preço médio por ativo;

quantidade total em carteira.

Módulo 3 – Métricas de Rentabilidade e Risco

Foco de estudo

Conceitos básicos:

rentabilidade simples x acumulada;

base percentual;

comparação com benchmarks.

Introdução a métricas de risco simples.

Impacto no FinTrack

Criar funções que:

calculem rentabilidade por ativo e consolidada em períodos definidos;

gerem uma tabela consolidada (posição, preço médio, rentabilidade, contribuição por ativo).

Preparar dados para visualização (tabelas “limpas” e agregadas).

Módulo 4 – Visualização de Dados (Python + JavaScript)

Foco de estudo

Visualização em Python (para prototipar):

gráficos básicos de linha, barra, pizza, scatter.

Visualização com JavaScript:

conceitos essenciais de DOM, dados e gráficos interativos.

inspiração no livro “Visualização de dados com Python e JavaScript”.

Impacto no FinTrack

Criar protótipos de gráficos:

evolução da carteira;

alocação por classe/setor;

contribuição por ativo.

Definir primeira versão de um painel simples (mesmo que estático) usando HTML + JS.

Módulo 5 – Organização, Testes e Entrega

Foco de estudo

Organização do projeto em pacotes/módulos.

Noções de testes automatizados (ex: pytest).

Documentação mínima e uso de requirements.txt.

Impacto no FinTrack

Refatorar o código para módulos mais claros (core, io, analytics, viz etc.).

Adicionar alguns testes automatizados para funções críticas (cálculo de preço médio, rentabilidade).

Revisar README e docs, preparando o projeto para ser usado como portfólio.