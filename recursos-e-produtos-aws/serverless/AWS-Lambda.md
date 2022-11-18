
Serviço que executa funções serverless, com características:
- Tem que informar linguagem e handler (função principal)
- Temos como configurar Layers, que podem ser customizados ou da própria AWS (cada um sua maneira de usar).
    - Layers são códigos adicionais aos lambdas, como se fosse bibliotecas ou containers paralelos
- Alias podem gerar novas function URL e vincular a versões publicadas
- Gatilhos podem ser criados para monitorar e invocar lambdas por eventos externos
- Eventos de saída dos lambdas podem notificar destino da função
