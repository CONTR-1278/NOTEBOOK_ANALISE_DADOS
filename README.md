# Análise de Dados - SOFTEX

## 📋 Descrição

Este projeto visa explorar os dados do primeiro lote enviado pela SOFTEX, realizando ETL (Extract, Transform, Load), primeiros insights, visualizações gráficas e geração de relatórios automatizados.

## 🎯 Objetivos

- **ETL**: Processamento e normalização dos dados brutos
- **Análise Exploratória**: Primeiros insights sobre os dados
- **Visualização**: Criação de gráficos e dashboards
- **Relatórios**: Geração automática de relatórios em Word
- **Modelo de Dados**: Criação de banco relacional normalizado

## 🛠️ Tecnologias

- **Python**: 3.10
- **Pandas**: Manipulação e análise de dados
- **SQLAlchemy**: ORM e banco de dados
- **Matplotlib/Seaborn**: Visualizações
- **Plotly**: Gráficos interativos
- **python-docx**: Geração de relatórios Word
- **PyPDF2**: Leitura de arquivos PDF
- **Graphviz**: Diagramas de relacionamento
- **Eralchemy2**: Modelo Entidade-Relacionamento
- **Geobr**: Dados geográficos do Brasil

## 📁 Estrutura do Projeto

```
NOTEBOOK_ANALISE_DADOS/
├── ANALISE_DE_DADOS/
│   ├── ANALISE_DADOS.ipynb          # Notebook principal
│   └── banco_de_dados_cntr_1278.db  # Banco SQLite gerado
├── RODADA 1 - Computador na atividade profissional/
│   ├── Cópia de Cópia de Base de dados - formato CSV.csv
│   └── Cópia de Cópia de Livro_de_codigos_assinado.pdf
├── images/                          # Gráficos e diagramas gerados
├── env/                             # Ambiente virtual Python
├── requirements.txt                 # Dependências do projeto
└── README.md                        # Este arquivo
```

## 📋 Pré-requisitos

### Documentos Necessários

**IMPORTANTE**: Coloque os documentos de cada lote da SOFTEX no mesmo nível do projeto:

- `ANALISE_DE_DADOS/` (pasta do notebook)
- `RODADA 1 - Computador na atividade profissional/` (pasta com dados)
- `RODADA 2 - .../` (próximos lotes)
- etc.

### Estrutura Esperada dos Dados

Cada pasta de rodada deve conter:
- Arquivo CSV com os dados da pesquisa
- Arquivo PDF com o dicionário de variáveis

## 🚀 Instalação e Configuração

### Linux

```bash
# Desativar ambiente virtual anterior (se existir)
deactivate

# Remover ambiente virtual anterior
rm -rf env

# Criar novo ambiente virtual
virtualenv -p /usr/bin/python3.10 env

# Ativar ambiente virtual
source env/bin/activate

# Atualizar pip
pip install --upgrade pip

# Instalar dependências via requirements.txt
pip install -r requirements.txt
```

### Windows

```cmd
# Desativar ambiente virtual anterior (se existir)
deactivate

# Remover ambiente virtual anterior
rmdir /s env

# Criar novo ambiente virtual
python -m venv env

# Ativar ambiente virtual
env\Scripts\activate

# Atualizar pip
python -m pip install --upgrade pip

# Instalar dependências via requirements.txt
pip install -r requirements.txt
```

### macOS

```bash
# Desativar ambiente virtual anterior (se existir)
deactivate

# Remover ambiente virtual anterior
rm -rf env

# Criar novo ambiente virtual
python3.10 -m venv env

# Ativar ambiente virtual
source env/bin/activate

# Atualizar pip
pip install --upgrade pip

# Instalar dependências via requirements.txt
pip install -r requirements.txt
```

## 📦 Instalação via Requirements

Alternativamente, você pode instalar todas as dependências de uma vez:

```bash
# Ativar ambiente virtual
source env/bin/activate  # Linux/macOS
# ou
env\Scripts\activate     # Windows

# Instalar via requirements.txt
pip install -r requirements.txt
```

## 🎯 Como Usar

1. **Configure o ambiente** seguindo as instruções de instalação acima
2. **Organize os dados** conforme a estrutura de pastas descrita
3. **Execute o notebook**:
   ```bash
   jupyter notebook ANALISE_DE_DADOS/ANALISE_DADOS.ipynb
   ```
4. **Selecione o kernel correto**: Use o kernel `env` (ambiente virtual)
5. **Execute as células** em sequência para gerar:
   - Banco de dados normalizado
   - Gráficos e visualizações
   - Relatórios em Word

## 📊 Saídas Geradas

- **Banco de Dados**: `banco_de_dados_cntr_1278.db` (SQLite)
- **Gráficos**: Pasta `images/` com visualizações
- **Relatórios**: Arquivos Word com análises
- **Diagramas**: MER (Modelo Entidade-Relacionamento)

## 🔧 Troubleshooting

### Erro de Kernel no Jupyter
Se o notebook não encontrar os módulos:
1. Vá em **Kernel** → **Change kernel**
2. Selecione o kernel `env`
3. Reinicie o kernel se necessário

### Erro de Módulos
Se algum módulo não for encontrado:
```bash
source env/bin/activate
pip install nome_do_modulo
```

## 📝 Licença

Este projeto foi desenvolvido para análise de dados da SOFTEX.

## 👥 Contribuição

Para contribuir com o projeto:
1. Faça um fork do repositório
2. Crie uma branch para sua feature
3. Commit suas mudanças
4. Push para a branch
5. Abra um Pull Request

## 📞 Suporte

Para dúvidas ou problemas, consulte a documentação ou entre em contato com a equipe de desenvolvimento.