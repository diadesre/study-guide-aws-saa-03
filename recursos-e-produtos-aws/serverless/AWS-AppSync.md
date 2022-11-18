# O que é
O AWS App Sync conecta com algumas fontes de dados (tanto de database quando de API [ex. AWS API de Lambda]) e transforma o conteúdo em GraphQL

# Como usar
Você conectar os schemas via GraphQL fazendo queries por meio de apps externos como JS, Android ou iOS. Os dados ficam salvo no dynamoDB (ou outra base escolhida)
Tem como fazer query também via console ou editar o schema pelo próprio console.

# Diferença entre REST API e GraphQL
A ideia do RestAPI trazer a inteligência e critérios a partir do backend por meio de uma ou mais requisições de API (baseado em comunicação de rede). O GraphQL permite que as consultas sejam instrumentadas a partir de queries em uma única chamada, informando as parametrizações necessárias.
O AppSync facilita essa jornada, entregando como serviço o endpoint GraphQL, conectando em fontes de origem diversas.

A REST API is an "architectural concept" for network-based software. GraphQL, on the other hand, is a query language and a set of tools that operate over a single endpoint. 
['See the reference'](https://hygraph.com/blog/graphql-vs-rest-apis)