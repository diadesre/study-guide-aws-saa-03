# Declaração de tarefa 1: Projetar acesso seguro aos recursos da AWS. 

- [Done] Aplicar as práticas recomendadas de segurança da AWS a usuários do IAM e usuários-raiz (por
exemplo, autenticação com multifator [MFA]). 

- Projetar um modelo de autorização flexível que inclua usuários, grupos, funções e políticas do IAM.

- [Done] Projetar uma estratégia de controle de acesso baseada em função (por exemplo, AWS Security Token Service [AWS STS], mudança de função, acesso entre contas).

Vale ressaltar que o uso de assume roles nos possibilitar segregar acessos sem conflitar o o privilégio que um ou outro grupo poderia ser superior. Exemplo, tem como testar acessos menores caso faça assume role ao invés de manter um mesmo usuário com mais de uma permissão vinculada a ele (via grupo ou direct attach).

- Projetar uma estratégia de segurança para várias contas da AWS (por exemplo, AWS Control
Tower, políticas de controle de serviço [SCPs]).
-- AWS Organizations
--- AI Services opt-out policy:
    Restringe o compartilhamento de resultados gerados por recursos de AI como serviço da AWS, ou seja, a amazon não usa os nossos resultados para melhorar os serviços deles
--- Política de Backup:
    Define planos com base na organization, para realizar backups com retenções definidas e aplicadas a recursos com padrões orientados a Tags e não necessariamente serviços específicos (ex.: somente para RDS)
--- SCPs: 
    Definem recursos ativados ou não em contas que estejam nas organizations. Caso não liberadas no IAM Policy da conta, o serviço é desabilitado.
--- Tag Policies:
    Definem critérios de uso das tags para todas as contas das organizations. No caso, podemos utilizar restrição de tamanho das letras (ex.: minúscula), definir valores esperados para a tag (Só pode valor X, Y ou Z) e também forçar que determinado recurso possua essa tag.
-- Control Tower
--- Temos que criar novas contas para fazer vinculo com as contas de Audit e Log Archive. 

- Determinar o uso apropriado de políticas de recursos para os serviços da AWS.
- Determinar quando federar um serviço de diretório com funções do IAM
