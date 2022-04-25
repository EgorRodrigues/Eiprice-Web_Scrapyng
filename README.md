### Prezado Candidato,
Agradeço o interesse de conhecer e poder compartilhar um pouco dos nossos desafios,
torcemos muito para que venha a contribuir na equipe, e juntos criarmos uma solução que
agregue impactos positivos para o Varejo / Indústria.

### Informações adicionais
Aqui na Eiprice buscamos pessoas que se identifiquem com nossa cultura.

### Temos 3 pilares principais:
Tecnologia e conhecimento são o nosso DNA: somos protagonistas do nosso
desenvolvimento, buscamos constantemente novos conhecimentos e os aplicamos em nossos
negócios e tecnologias.

O sucesso do cliente é o nosso sucesso: os nossos clientes estão no centro de todas as
decisões. Temos empatia e buscamos soluções que gerem valor ao seu negócio.

Valorizamos gente boa que é boa gente: somos inquietos, questionadores e inconformados.
Temos foco em resultados de excelência, trabalhando em um ambiente de constantes
mudanças, desafios e colaboração.

### Avaliação Técnica
Criar um web scraping para extração de dados no shopper, este script permite consultar todos
os dados do departamento Alimentos assim como seus níveis
Ex: Categorias, Subcategorias caso estejam presentes
BASE URL: https://unica.shopper.com.br/shop/#bemvindo
DEPARTAMENTO: Alimentos
obs:
- Caso o script apresente uma falha inesperada o mesmo deve permitir voltar do estado
atual.

Layout do arquivo assortment.csv:


| Coluna(s)  | Descrição                                       | Valor                                                                                        | Tipo    |
|------------|-------------------------------------------------|----------------------------------------------------------------------------------------------|---------|
| name       | Nome do produto                                 | Vegan crunchy bar caramelo e cacau bio2 28g                                                  | string  |
| sku        | Código Interno do produto                       | 11180                                                                                        | string  |
| department | Departamento                                    | Natureba                                                                                     | string  |
| category   | Categoria                                       | Frutas secas e barrinhas                                                                     | string  |
| url        | Url do produto                                  | https://programada.shopper.com.br/shop/destaques/vegan-crunchy-bar-caramelo-e-cacau-bio2-28g | string  |
| image      | Imagem do produto                               | https://d2om08pcbtz1n1.cloudfront.net/be757786-114c-4d15-8669-c8a804604ffd.jpg               | string  |
| price_to   | Preço por                                       | 3.99                                                                                         | numeric |
| discount   | Desconto do produto                             | 15%                                                                                          | string  |
| available  | S = Produto Disponível N = Produto Indisponível | S                                                                                            | string  |
| stock_qty  | Qtde de Estoque do produto                      | 5                                                                                            | numeric |
| store      | Loja Principal                                  | Shopper                                                                                      | string  |
| created_at | Data da captura                                 | 2021-09-30                                                                                   | date    |
| hour       | Hora da captura                                 | 14:47:25                                                                                     | time    |


#### Layout do arquivo seller.csv:

| Coluna(s)      | Descrição                                       | Valor                                                                                        | Tipo    |
|----------------|-------------------------------------------------|----------------------------------------------------------------------------------------------|---------|
| name           | Nome do produto                                 | Acucar cristal organico native sache 250g                                                    | string  | 
| sku            | Código Interno do produto                       | 1795                                                                                         | string  |
| department     | Departamento                                    | Alimentos                                                                                    | string  |
| category       | Categoria                                       | Acucar e adocantes                                                                           | string  |
| seller_store   | Loja Principal                                  | Shopper                                                                                      | string  |
| seller_player  | Vendedor (Loja utilizada como métrica de preço) | Sonda                                                                                        | string  |
| price_store    |                                                 | 4.99                                                                                         | numeric |
| price_player   |                                                 | 6.04                                                                                         | numeric |
| discount_store | Desconto do produto                             | 29%                                                                                          | string  |
| available      | S = Produto Disponível N = Produto Indisponível | S                                                                                            | string  |
| stock_qty      | Qtde de Estoque do produto                      | 5                                                                                            | numeric |
| url            | Url do produto                                  | https://programada.shopper.com.br/shop/destaques/vegan-crunchy-bar-caramelo-e-cacau-bio2-28g | string  |
| image          | Imagem do produto                               | https://d2om08pcbtz1n1.cloudfront.net/be757786-114c-4d15-8669-c8a804604ffd.jpg               | string  |
| created_at     | Data da captura                                 | 2021-09-30                                                                                   | date    |
| hour           | Hora da captura                                 | 14:47:25                                                                                     | time    |

| Serviços          | Descrição                                                                                                | Requisitos |
|-------------------|----------------------------------------------------------------------------------------------------------|------------|
| Back End          | Python >= 3.9                                                                                            | Sim        |
| Banco Dados       | Postgres >= 11                                                                                           | Sim        |
| APIs              | Fast API:<br/> - Visão Assortment <br/>- Visão Seller <br/><br/>Plus: opções de filtros <br/>Ex: por sku | Plus       |
| Script Exportação | Relatório(s) consolidados com os layout definidos acima: assortment.csv seller.csv                       | Sim        |

**Prazo Entrega:** 3 dias após o envio do teste <br>
**Repositórios para entrega dos dados:** Git Lab, Bitbucket ou Github
