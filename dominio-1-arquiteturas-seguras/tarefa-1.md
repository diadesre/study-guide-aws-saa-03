# Declaração de tarefa 1: Projetar acesso seguro aos recursos da AWS. 

- [Done] Aplicar as práticas recomendadas de segurança da AWS a usuários do IAM e usuários-raiz (por
exemplo, autenticação com multifator [MFA]). 

- Projetar um modelo de autorização flexível que inclua usuários, grupos, funções e políticas do IAM.

- [Done] Projetar uma estratégia de controle de acesso baseada em função (por exemplo, AWS Security
Token Service [AWS STS], mudança de função, acesso entre contas). -> 

Vale ressaltar que o uso de assume roles nos possibilitar segregar acessos sem conflitar o o privilégio que um ou outro grupo poderia ser superior. Exemplo, tem como testar acessos menores caso faça assume role ao invés de manter um mesmo usuário com mais de uma permissão vinculada a ele (via grupo ou direct attach).

- Projetar uma estratégia de segurança para várias contas da AWS (por exemplo, AWS Control
Tower, políticas de controle de serviço [SCPs]).

- Determinar o uso apropriado de políticas de recursos para os serviços da AWS.
- Determinar quando federar um serviço de diretório com funções do IAM
