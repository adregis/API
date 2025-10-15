# Generic 3scale GitOps

O repositório `generic` foi criado com o objetivo de fornecer aos administradores do 3scale um controle completo e altamente personalizável sobre os Custom Resources (CRs) utilizados na plataforma. Este repositório adota uma abordagem baseada em Helm Charts, permitindo flexibilidade na configuração e automação dos seguintes recursos:

- Application
- Backend
- DeveloperAccount
- DeveloperUser
- Product
- ActiveDoc

A estrutura do repositório foi projetada para ser a base de outros repositórios específicos, ou seja, **todos os novos repositórios podem e preferencialmente devem ser derivados deste**. Ele já contém uma estrutura inicial e genérica que pode ser adaptada conforme necessário, reduzindo a duplicação de código e facilitando a padronização. Essa estrutura inclui diretórios e arquivos organizados de forma lógica, como `templates`, `values`.

Os arquivos de values deste repositório permitem um controle total sobre as `metadatas` e as `specs` dos Custom Resources (CRs). Por exemplo, o arquivo de values para a criação de um Backend pode ser configurado da seguinte forma:

Este nível de personalização exige **conhecimento técnico avançado** dos administradores do 3scale, que devem entender profundamente a estrutura e a semântica dos Custom Resources do produto, de acordo com a documentação do Operator
