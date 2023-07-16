# Prevenção de Churn

Neste projeto, a partir do dataset obtido no kaggle (que pode ser encontrado [aqui](https://www.kaggle.com/datasets/radheshyamkollipara/bank-customer-churn)) será feito uma análise de churn, no primeiro momento fazendo uma análise exploratória para verificar quais os principais atributos que levam o cliente a desistência e também construir um modelo que classifique se o cliente irá desistir ou não.

O intuito com esse projeto é tratar com *classes desbalanceados* de acordo com o capítulo 9 do livro **Machine learning Guia de Referência Rápida** (este livro pode ser encontrado na amazon [aqui](https://www.amazon.com.br/Machine-Learning-Refer%C3%AAncia-Trabalhando-Estruturados/dp/857522817X)) já que a classes com churn é muito maior do que as pessoas sem.

## Dicionário dos dados

O dataset vem com 18 atributos, sendo eles:

- **RowNumber**: Corresponde ao número da linha
- **CustomerId**: número de ID do cliente
- **Surname**: o apelido de um cliente
- **CreditScore**: Score de crédito do cliente
- **Geography**: Pais onde o cliente reside
- **Gender**: Genero do cliente
- **Age**: Idade do cliente
- **Tenure**: Refere-se ao número de anos que o cliente tem sido cliente do banco
- **Balance**: Balanço no cartão de crédito
- **NumOfProducts**: Número de produtos que o cliente comprou através do banco
- **HasCrCard**: Se tem ou não um cartão de crédito
- **IsActiveMember**: Se o cliente é ativo
- **EstimatedSalary**: Salário estimado do cliente
- **Exited**: Se o cliente deixou ou não o banco (*este será a nossa variável target*)
- **Complain**: Cliente tem alguma reclamação ou não
- **Satisfaction Score**: Pontuação fornecida pelo cliente para resolução de sua reclamação.
- **Card Type**: Tipo de cartão em posse do cliente.
- **Point Earned**: Pontos que o cliente adquiriu pelo uso do cartão de crédito

Observa-se que as três primeira colunas não são necessária nem para a análise nem para modelagem, logo elas foram desconsideradas, logo só se trabalhará com as 15 restantes.

## Análise Exploratória
