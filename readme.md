## ------- Projeto de análise descritiva e tratamento de dados -------

De modo geral, é possível afirmar que dados são conjuntos de informações (ocorrências) e valores que, ao serem comparados e combinados, podem gerar bases complexas de conhecimentos e propiciar grandes benefícios financeiros e intelectuais aos seus detentores.

Nesse sentido, considere que você é um cientista de dados em uma grande empresa familiar do ramo imobiliário.

## --------------

- Você recebeu a tarefa de projetar uam visualização de dados sobre os resultados financeiros do último trimestre do ano, considerando os pagamentos de aluguéis e os inadimplentes do período.

- Os dados serão obtidos de diversas fontes, como planilhas, planilhas excel e relatórios extraídos do sistema web da empresa.

- Tendo em vista que seu público alvo não tem um perfil técnico, você sente a necessidade de simplificar as informações ao máximo, de modo a não gerar grandes dificuldades na compreensão dos dados.

- Metade da equipe gestora tem domínio básico de informática e a outra metade tem conhecimentos intermediários de excel.

## --------------

### -- OBS--> O cliente forneceu apenas uma planilha excel com poucas informações. sendo possível apresentar apenas dados estatísticos dos juros cobrados e dos aluguéis cobrados.

### Responda:

###### a) Levando em conta que a visualização de dados deve ser projetada para um público não técnico, quais ferramentas podem ser adotadas para a projeção dos resultados financeiros da imobiliária?

###### **R - Acredito que WORD CLOUDS não seria interessante pois a demanda é a de apresentação de resultados estatísticos. A ferramenta ideal para essa atividade seria a apresentação de gráficos onde serão informados os dados de acordo com cada mês.**

###### b) Como você projetaria visualmente os dados de inadimplentes e pagantes do último trimestre do ano? Identifique e detalhe possíveis soluções, justificando-as.

###### **R - através De um gráfico de colunas. Acredito que seria suficiente para um simples entendimento do relatório.**

###### c) Com base no arquivo DadosDesafio.xlsx, apresente um código ​​​​​​​em Python mostrando a carga dos dados e, em seguida, demonstre a **média** e os valores **mínimos** e **máximos** de cada coluna numérica da planilha.

###### **R - considerando que a coluna cod_imovel não necessita de dados estatístico pois é apenas um ID, o dia de vencimento é um parâmetro e as datas mostram se o serviço foi pago em dia ou não, só podemos apresentar esses dados estatísticos do valor do aluguel e da porcentagem de juros visto que aparentemente, o juros reflete o atraso referente ao trimestre e não ao mês ou dia de atraso. Faltam informações para análises mais precisas. Portanto, serão apresentados os dados estatísticos dos alugueis cobrados e dos juros cobrados(considerando que seu valor total se refere a todo o trimestre).**
