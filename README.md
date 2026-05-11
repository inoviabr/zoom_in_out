# Tutorial — post Medium

Repositório com o notebook de apoio ao artigo no Medium: experimentos com **PyTorch**, **torchvision** e o conjunto de dados **PCam** (classificação de patches em imagens histopatológicas).

## Pré-requisitos

- Python 3.10 ou superior (recomendado 3.12)
- `pip`

## Configuração do ambiente

1. Clone ou copie este repositório para a sua máquina.

2. Crie e ative um ambiente virtual:

   ```bash
   python3 -m venv venv
   source venv/bin/activate   # Linux/macOS
   # ou: venv\Scripts\activate  no Windows
   ```

3. Instale as dependências usadas no notebook (exemplo):

   ```bash
   pip install torch torchvision matplotlib tqdm
   ```

   Outros pacotes podem ser necessários conforme as células do notebook (por exemplo `gdown`, `beautifulsoup4`, etc.).

## Como usar

1. Ative o `venv` como acima.
2. Abra o Jupyter (ou VS Code / Cursor com suporte a notebooks) e execute `code.ipynb` célula a célula.

O notebook faz download do **PCam** para a pasta `data/` na primeira execução; o download é grande — reserve espaço em disco e conexão estável.

## Estrutura

| Item | Descrição |
|------|-----------|
| `code.ipynb` | Tutorial interativo (instalação, imports, carregamento do PCam, etc.) |
| `data/` | Dados baixados pelo torchvision (ignorado pelo Git; ver `.gitignore`) |
| `venv/` | Ambiente virtual local (não versionado) |

## Licença e dados

Respeite os termos de uso do **PCam** / **Camelyon** e das bibliotecas citadas no notebook. Este repositório contém apenas código e notas de tutorial; os pesos e datasets não são incluídos no Git.
