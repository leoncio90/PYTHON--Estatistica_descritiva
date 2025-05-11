# PYTHON--Estatistica_descritiva: Projeto de Tratamento, Análise e Relatório de Dados

Este projeto demonstra um fluxo completo de trabalho com dados utilizando Python, focado no tratamento e limpeza de um conjunto de dados brutos, realização de análises estatísticas descritivas e, por fim, na geração de um relatório consolidado em formato Excel com visualizações.

O principal artefato deste repositório é o notebook Jupyter `elaborando_relatorio.ipynb`, que detalha cada etapa do processo.

## Objetivos do Projeto

* Realizar uma limpeza e transformação abrangente em um conjunto de dados (originalmente de um arquivo Excel).
* Aplicar técnicas de engenharia de atributos para extrair informações relevantes.
* Calcular estatísticas descritivas básicas (média, mínimo, máximo) para colunas financeiras chave.
* Gerar visualizações (gráficos de barras) para representar essas estatísticas.
* Produzir um relatório final em Excel contendo os dados tratados e as visualizações geradas.

## Funcionalidades Implementadas

O notebook `elaborando_relatorio.ipynb` executa as seguintes etapas:

1.  **Carregamento de Dados:**
    * Leitura do arquivo de entrada `dadosDesafio.xlsx` utilizando a biblioteca Pandas.

2.  **Limpeza e Pré-processamento Extensivo dos Dados**:
    * Padronização dos nomes das colunas (maiúsculas, snake_case, remoção de acentos, substituição de abreviações).
    * Limpeza de dados textuais (remoção de espaços, normalização de acentos, conversão para maiúsculas, substituição de "AV." por "AVENIDA").
    * Conversão de tipos de dados para formatos apropriados (strings, floats, datas).
    * Tratamento específico de datas e formatação da coluna `DIA_VENCIMENTO`.

3.  **Engenharia de Atributos**:
    * Extração do número do imóvel a partir da coluna de endereço usando expressões regulares (`re.search(r'\d+$', ENDERECO_IMOVEL)`), criando uma nova coluna `NUMERO_IMOVEL` e atualizando a coluna `ENDERECO_IMOVEL`.

4.  **Análise Estatística Descritiva**:
    * Cálculo da média, valor mínimo e valor máximo para as colunas `ALUGUEL` e `JUROS_ATRASO`.

5.  **Visualização de Dados**:
    * Criação de gráficos de barras com Matplotlib para apresentar as estatísticas de `ALUGUEL` e `JUROS_ATRASO`.
    * Salvamento dos gráficos como arquivos PNG (`grafico_aluguel.png` e `grafico_juros.png`).

6.  **Geração de Relatório**:
    * Criação de um arquivo Excel (`Relatório_Trimestral.xlsx`) utilizando Openpyxl.
    * Incorporação dos gráficos PNG gerados em uma planilha dentro do relatório Excel.
    * Salvamento do DataFrame com os dados já tratados e limpos no arquivo `dadosTratados.xlsx`.

## Tecnologias Utilizadas

* **Python 3**
* **Jupyter Notebook**
* **Bibliotecas Python:**
    * **Pandas:** Para manipulação e análise de dados tabulares.
    * **NumPy:** (Utilizado indiretamente pelo Pandas) Para operações numéricas.
    * **Matplotlib:** Para a criação de gráficos e visualizações.
    * **Openpyxl:** Para leitura e escrita de arquivos Excel (.xlsx).
    * **re (Expressões Regulares):** Para manipulação avançada de strings.
    * **datetime:** Para manipulação de datas.
    * **os:** (Utilizado para interações com o sistema de arquivos, se necessário para caminhos de arquivos).

## Pré-requisitos

Para executar este projeto, você precisará ter o Python 3 instalado, juntamente com as bibliotecas listadas acima. Você pode instalá-las usando pip:

```bash
pip install pandas matplotlib openpyxl jupytergit push origin main