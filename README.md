# FinTrack

FinTrack é um painel de análise de carteira de investimentos em construção, usado como projeto-guia do meu “curso pessoal” de Ciência de Dados.

A ideia é evoluir o FinTrack módulo a módulo, enquanto estudo Python, bibliotecas de dados e visualização com JavaScript. No final, quero ter uma ferramenta capaz de:

- Importar operações de investimentos (arquivos da corretora, planilhas etc.).
- Calcular posição atual da carteira.
- Calcular preço médio.
- Calcular rentabilidade (por ativo e consolidada).
- Analisar alocação da carteira (setores, classes de ativos, risco x retorno).
- Gerar visualizações interativas.

---

## 🔧 Stack inicial

- **Linguagem principal:** Python 3.12  
- **Ambiente:** `venv` (ambiente virtual por projeto)  
- **Ferramentas de desenvolvimento:**
  - VS Code (editor/IDE principal)
  - Jupyter Notebooks (exploração de dados, protótipos)
- **Bibliotecas Python (mínimo atual):**
  - `pandas` – manipulação de dados tabulares
  - `jupyter` – notebooks interativos

> Mais bibliotecas serão adicionadas ao longo dos módulos (visualização, finanças, APIs etc.).

---

## 🗂 Estrutura do projeto (inicial)

```text
fintrack/
  .venv/                # ambiente virtual (não versionado)
  data/
    raw/                # dados brutos (notas de corretagem, planilhas, etc.)
    processed/          # dados tratados / intermediários
  notebooks/            # experimentos e exploração de dados
  fintrack/
    __init__.py         # transforma a pasta em pacote Python
    main.py             # ponto de entrada inicial do projeto
  tests/                # futuros testes automatizados
  docs/                 # documentação (roadmap, anotações, etc.)
  .gitignore            # arquivos/pastas que não serão versionados
  requirements.txt      # dependências do projeto
  README.md             # este arquivo
```
## ▶️ Como rodar o projeto localmente

### ✅ Pré-requisitos

- Python 3.12 instalado e acessível via terminal:
  
  ```bash
  python --version

- Git instalado:

  ```bash
  git --version

1. Clonar o repositório
   ```bash
   git clone https://github.com/riomarfilho/fintrack.git
   cd fintrack

2. Criar e ativar o ambiente virtual
   
   ```bash
   python -m venv .venv
    .\.venv\Scripts\Activate.ps1

Se der certo, o terminal deve mostrar algo como:
   ```bash
   (.venv) PS C:\Users\...\fintrack>
```
3. Instalar dependências

Com o ambiente virtual ativo:
   ```bash
    pip install -r requirements.txt
```
4. Testar se o FinTrack “levanta”

```bash
    python -m fintrack.main



