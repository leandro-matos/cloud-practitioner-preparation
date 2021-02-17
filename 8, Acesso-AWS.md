
## AWS Management Console (HTTP)
 - Interface gráfica via browser;

## COmmand Line Interface (CLI)
 - Acesso root das instâncias e controlar múltiplos serviços;

## Software Development Kit (SDK)
 - Acesso via API utilizando linguagens de programação (Python, php, node, etc);

## TOP 10 Perguntas Frequentes IAM

### 1. O que é um usuário?

Um usuário é uma identidade exclusiva reconhecida pelos serviços e aplicativos da AWS. Semelhante a um usuário de login em um sistema operacional do Windows ou UNIX, este é um usuário com um nome exclusivo e pode se identificar usando credenciais de segurança familiares, como uma senha ou chave de acesso. O usuário pode ser um indivíduo, um sistema ou um aplicativo que precise de acesso aos serviços da AWS. O IAM oferece suporte para usuários gerenciados no sistema de gerenciamento de identidades da AWS (chamados de "usuários do IAM") e também permite que você conceda acesso a recursos da AWS para usuários gerenciados fora da AWS em seu diretório corporativo (chamados de "usuários federados").

### 2. O que é um grupo?
Um grupo é um conjunto de usuários do IAM, possuindo as seguintes características:

Podendo adicionar usuários ou remover de um grupo.

Um usuário pode pertencer a vários grupos.

Os grupos não podem pertencer a outros grupos.

Os grupos podem obter permissões usando políticas de controle de acesso. Isso facilita o gerenciamento de permissões para um conjunto de usuários, em vez de ter de gerenciar permissões para cada usuário individual.

Os grupos não têm credenciais de segurança e não podem acessar serviços da Web diretamente; eles existem somente para facilitar o gerenciamento de permissões de usuários.

### 3. Posso habilitar e desabilitar o acesso de um usuário?

Sim. Você pode habilitar e desabilitar a chaves de acesso de um usuário do IAM por meio de APIs do IAM, da CLI da AWS ou do console do IAM. Se você desabilitar as chaves de acesso, o usuário não poderá acessar programaticamente os serviços da AWS.

### 4. Posso estruturar um grupo de usuários de modo hierárquico, assim como no LDAP?
Sim. Você pode organizar usuários e grupos em caminhos, semelhantes a caminhos de objetos no Amazon S3 – por exemplo, minhaempresa/area/projeto/joao.

### 5. Posso definir usuários regionalmente?
Não. Os usuários são entidades globais, como uma conta da AWS é hoje. Nenhuma região precisa ser especificada quando você define permissões do usuário. Os usuários podem usar serviços da AWS em qualquer região geográfica.

### 6. Os nomes de usuários do IAM têm de ser endereços de e-mail?

Não, mas podem ser. Os nomes de usuário são apenas strings ASCII que são exclusivas dentro de uma determinada conta da AWS. Você pode atribuir nomes usando qualquer convenção de nomes que escolher, incluindo endereços de e-mail.

### 7. Posso definir uma política para as senhas dos meus usuários?

Sim, você pode aplicar senhas fortes, como senhas com comprimento mínimo ou com pelo menos um número. Você também pode aplicar expiração automática de senhas, impedir a reutilização de senhas antigas e exigir a redefinição da senha no próximo login na AWS.

### 8. O que é uma função (ROLE) do IAM?

Uma função (ROLE) é uma entidade do IAM que define um conjunto de permissões para efetuar solicitações de serviços da AWS. As funções do IAM não são associadas a um usuário ou grupo específico. Em vez disso, entidades de confiança assumem funções, como usuários do IAM, aplicativos ou serviços da AWS, como o EC2.

### 9. Como funcionam as permissões?

As políticas de controle de acesso são anexadas a usuários, grupos e funções para atribuir permissões a recursos da AWS. Por padrão, os usuários, grupos e funções do IAM não têm permissões. Usuários com permissões suficientes devem usar uma política para conceder as permissões desejadas.

### 10. O que é o AWS MFA?

O AWS Multi-Factor Authentication (conhecido como autenticação de duas etapas) fornece um nível extra de segurança que pode ser aplicado ao seu ambiente AWS. É possível habilitar o AWS MFA para a sua conta AWS e para usuários individuais do AWS Identity and Access Management (IAM) que você cria em sua conta.


Quer se aprofundar? https://aws.amazon.com/pt/iam/faqs/
