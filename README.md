📊 Pipeline de Dados: Combinando Python e Orientação a Objetos
Projeto desenvolvido durante o curso "Pipeline de Dados: Combinando Python e Orientação a Objetos".
Este repositório contém um exemplo prático de um pipeline ETL (Extração, Transformação e Carga) implementado em Python utilizando orientação a objetos. 

📘 Sobre o Projeto
O objetivo deste projeto é unir dados provenientes de duas fontes distintas:

Empresa A: dados no formato JSON
Empresa B: dados no formato CSV
Após a leitura dos arquivos, os dados são transformados (renomeando colunas e unindo as bases), e por fim salvos em um único arquivo CSV como parte do processo de carga (Load).

🧱 Estrutura do Projeto

pipeline-dados-empresaAB/
├── data_raw/                     # Dados brutos das empresas
│   ├── dados_empresaA.json       # Dados da empresa A (JSON)
│   └── dados_empresaB.csv        # Dados da empresa B (CSV)
│
├── data_processed/               # Dados processados após o pipeline
│   └── dados_combinados.csv      # Arquivo final combinado
│
├── processamento_dados.py        # Classe principal 'Dados' para manipulação dos dados
├── fusao_mercados_fev.py         # Script principal que executa o pipeline ETL
│
└── README.md                     # Este arquivo

profile
Qwen3-235B-A22B
9:38 am
Claro! Vou te ajudar a montar um README.md completo e bem estruturado para o seu repositório. Este arquivo será essencial para que outras pessoas entendam, usem e contribuam com o seu projeto.

Aqui está uma sugestão de conteúdo para o README.md, baseada nos scripts e no curso:

📊 Pipeline de Dados: Combinando Python e Orientação a Objetos
Projeto desenvolvido durante o curso "Pipeline de Dados: Combinando Python e Orientação a Objetos".
Este repositório contém um exemplo prático de um pipeline ETL (Extração, Transformação e Carga) implementado em Python utilizando orientação a objetos. 

📘 Sobre o Projeto
O objetivo deste projeto é unir dados provenientes de duas fontes distintas:

Empresa A: dados no formato JSON
Empresa B: dados no formato CSV
Após a leitura dos arquivos, os dados são transformados (renomeando colunas e unindo as bases), e por fim salvos em um único arquivo CSV como parte do processo de carga (Load).

🧱 Estrutura do Projeto
pipeline-dados-empresaAB/
├── data_raw/                     # Dados brutos das empresas
│   ├── dados_empresaA.json       # Dados da empresa A (JSON)
│   └── dados_empresaB.csv        # Dados da empresa B (CSV)
│
├── data_processed/               # Dados processados após o pipeline
│   └── dados_combinados.csv      # Arquivo final combinado
│
├── processamento_dados.py        # Classe principal 'Dados' para manipulação dos dados
├── fusao_mercados_fev.py         # Script principal que executa o pipeline ETL
│
└── README.md                     # Este arquivo
⚙️ Funcionalidades
Leitura automática de dados em formatos JSON ou CSV.
Renomeio flexível de colunas com mapeamento customizável.
Junção de múltiplas fontes de dados.
Salvamento em arquivo CSV organizado.
Implementação orientada a objetos para fácil manutenção e escalabilidade.
🛠️ Como Executar
1. Requisitos
Certifique-se de ter instalado:

Python 3.x
Ambiente virtual (recomendado)
Pacotes necessários: json, csv
2. Clonando o repositório

git clone https://github.com/seu-usuario/pipeline-dados-empresaAB.git 
cd pipeline-dados-empresaAB

3. Criando ambiente virtual (opcional mas recomendado)

python -m venv venv
source venv/bin/activate    # Linux/Mac
# ou
venv\Scripts\activate       # Windows

profile
Qwen3-235B-A22B
9:38 am
Claro! Vou te ajudar a montar um README.md completo e bem estruturado para o seu repositório. Este arquivo será essencial para que outras pessoas entendam, usem e contribuam com o seu projeto.

Aqui está uma sugestão de conteúdo para o README.md, baseada nos scripts e no curso:

📊 Pipeline de Dados: Combinando Python e Orientação a Objetos
Projeto desenvolvido durante o curso "Pipeline de Dados: Combinando Python e Orientação a Objetos".
Este repositório contém um exemplo prático de um pipeline ETL (Extração, Transformação e Carga) implementado em Python utilizando orientação a objetos. 

📘 Sobre o Projeto
O objetivo deste projeto é unir dados provenientes de duas fontes distintas:

Empresa A: dados no formato JSON
Empresa B: dados no formato CSV
Após a leitura dos arquivos, os dados são transformados (renomeando colunas e unindo as bases), e por fim salvos em um único arquivo CSV como parte do processo de carga (Load).

🧱 Estrutura do Projeto
pipeline-dados-empresaAB/
├── data_raw/                     # Dados brutos das empresas
│   ├── dados_empresaA.json       # Dados da empresa A (JSON)
│   └── dados_empresaB.csv        # Dados da empresa B (CSV)
│
├── data_processed/               # Dados processados após o pipeline
│   └── dados_combinados.csv      # Arquivo final combinado
│
├── processamento_dados.py        # Classe principal 'Dados' para manipulação dos dados
├── fusao_mercados_fev.py         # Script principal que executa o pipeline ETL
│
└── README.md                     # Este arquivo
⚙️ Funcionalidades
Leitura automática de dados em formatos JSON ou CSV.
Renomeio flexível de colunas com mapeamento customizável.
Junção de múltiplas fontes de dados.
Salvamento em arquivo CSV organizado.
Implementação orientada a objetos para fácil manutenção e escalabilidade.
🛠️ Como Executar
1. Requisitos
Certifique-se de ter instalado:

Python 3.x
Ambiente virtual (recomendado)
Pacotes necessários: json, csv
2. Clonando o repositório
bash
git clone https://github.com/seu-usuario/pipeline-dados-empresaAB.git 
cd pipeline-dados-empresaAB
3. Criando ambiente virtual (opcional mas recomendado)
bash
python -m venv venv
source venv/bin/activate    # Linux/Mac
# ou
venv\Scripts\activate       # Windows
4. Instalando dependências (nenhuma externa necessária neste projeto)
Este projeto utiliza apenas bibliotecas nativas do Python (json e csv), então não há necessidade de instalar pacotes adicionais. 

5. Baixando os dados (exemplo com wget)
Se ainda não tiver os arquivos, você pode baixá-los com:

mkdir -p data_raw

wget -O data_raw/dados_empresaA.json https://cdn3.gnarususercontent.com.br/3062-pipeline-dados/dados/dados_empresaB.csv 
wget -O data_raw/dados_empresaB.csv https://cdn3.gnarususercontent.com.br/3062-pipeline-dados/dados/dados_empresaA.json 

⚠️ Atenção: Confira se os links estão corretos e disponíveis.

6. Executando o pipeline

python fusao_mercados_fev.py

Após a execução, o arquivo dados_combinados.csv será criado na pasta data_processed.

📝 Exemplo de Saída
Será exibido no terminal:

['Nome do Produto', 'Categoria do Produto', 'Preço do Produto (R$)', ...]
Quantidade de linhas: X
...
Arquivo salvo em: data_processed/dados_combinados.csv

['Nome do Produto', 'Categoria do Produto', 'Preço do Produto (R$)', ...]
Quantidade de linhas: X
...
Arquivo salvo em: data_processed/dados_combinados.csv

profile
Qwen3-235B-A22B
9:38 am
Claro! Vou te ajudar a montar um README.md completo e bem estruturado para o seu repositório. Este arquivo será essencial para que outras pessoas entendam, usem e contribuam com o seu projeto.

Aqui está uma sugestão de conteúdo para o README.md, baseada nos scripts e no curso:

📊 Pipeline de Dados: Combinando Python e Orientação a Objetos
Projeto desenvolvido durante o curso "Pipeline de Dados: Combinando Python e Orientação a Objetos".
Este repositório contém um exemplo prático de um pipeline ETL (Extração, Transformação e Carga) implementado em Python utilizando orientação a objetos. 

📘 Sobre o Projeto
O objetivo deste projeto é unir dados provenientes de duas fontes distintas:

Empresa A: dados no formato JSON
Empresa B: dados no formato CSV
Após a leitura dos arquivos, os dados são transformados (renomeando colunas e unindo as bases), e por fim salvos em um único arquivo CSV como parte do processo de carga (Load).

🧱 Estrutura do Projeto
pipeline-dados-empresaAB/
├── data_raw/                     # Dados brutos das empresas
│   ├── dados_empresaA.json       # Dados da empresa A (JSON)
│   └── dados_empresaB.csv        # Dados da empresa B (CSV)
│
├── data_processed/               # Dados processados após o pipeline
│   └── dados_combinados.csv      # Arquivo final combinado
│
├── processamento_dados.py        # Classe principal 'Dados' para manipulação dos dados
├── fusao_mercados_fev.py         # Script principal que executa o pipeline ETL
│
└── README.md                     # Este arquivo
⚙️ Funcionalidades
Leitura automática de dados em formatos JSON ou CSV.
Renomeio flexível de colunas com mapeamento customizável.
Junção de múltiplas fontes de dados.
Salvamento em arquivo CSV organizado.
Implementação orientada a objetos para fácil manutenção e escalabilidade.
🛠️ Como Executar
1. Requisitos
Certifique-se de ter instalado:

Python 3.x
Ambiente virtual (recomendado)
Pacotes necessários: json, csv

2. Clonando o repositório
bash
git clone https://github.com/seu-usuario/pipeline-dados-empresaAB.git 
cd pipeline-dados-empresaAB
3. Criando ambiente virtual (opcional mas recomendado)
bash
python -m venv venv
source venv/bin/activate    # Linux/Mac
# ou
venv\Scripts\activate       # Windows
4. Instalando dependências (nenhuma externa necessária neste projeto)
Este projeto utiliza apenas bibliotecas nativas do Python (json e csv), então não há necessidade de instalar pacotes adicionais. 

5. Baixando os dados (exemplo com wget)
Se ainda não tiver os arquivos, você pode baixá-los com:

bash
mkdir -p data_raw

wget -O data_raw/dados_empresaA.json https://cdn3.gnarususercontent.com.br/3062-pipeline-dados/dados/dados_empresaB.csv 
wget -O data_raw/dados_empresaB.csv https://cdn3.gnarususercontent.com.br/3062-pipeline-dados/dados/dados_empresaA.json 
⚠️ Atenção: Confira se os links estão corretos e disponíveis.

6. Executando o pipeline
bash
python fusao_mercados_fev.py
Após a execução, o arquivo dados_combinados.csv será criado na pasta data_processed.

📝 Exemplo de Saída
Será exibido no terminal:

['Nome do Produto', 'Categoria do Produto', 'Preço do Produto (R$)', ...]
Quantidade de linhas: X
...
Arquivo salvo em: data_processed/dados_combinados.csv
📌 O que foi aprendido?
Como organizar um projeto de engenharia de dados;
Manipulação de dados em JSON e CSV;
Uso de classes e orientação a objetos para modularização;
Criação de um pipeline ETL simples e eficiente;
Práticas de refatoração e encapsulamento.

💬 Contato
Se quiser compartilhar feedbacks, melhorias ou dúvidas:

Diêgo Lima
www.linkedin.com/in/nascimento-jdl
