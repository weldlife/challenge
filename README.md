# Desafio
Construa uma API, que responda JSON, para utilização de cupons. Está aplicação é uma coleção de códigos (cupons) que podem ser usados pelos clientes (destinatários) para obter descontos em uma loja virtual.

Cada código pode ser usado apenas uma vez e gostaríamos de saber quando foi usado pelo destinatário.

Como pode haver muitos destinatários, precisamos de uma chamada que gere automaticamente códigos de comprovante para cada destinatário.

Infomaçes gerais sobre as entidades

Destinatário
- Nome
- Email (exclusivo)

Oferta Especial
- Nome
- Desconto percentual fixo

Cupom
- Código exclusivo gerado aleatoriamente (pelo menos 8 caracteres)
- atribuído a um destinatário e a uma oferta especial
- Data de validade
- Pode ser usado apenas uma vez
- Deve rastrear a data de uso

Funcionalidades
1) Para uma determinada Oferta Especial e uma data de vencimento, gere um código para cada destinatário 
2) Para um determinado e-mail, devolva todos os seus códigos válidos com o nome do Oferta Especial
3) Para um determinado e-mail e cdigo, caso o cdigo seja válido, retorne o desconto percentual e defina o data de uso

( opcional ) Criar uma paǵna para consumo das APIs

## Requisitos
- Forkar esse desafio e criar o seu projeto (ou workspace) usando a sua versão desse repositório, tão logo acabe o desafio, submeta um pull request.
- Caso você tenha algum motivo para não submeter um pull request, crie um repositório privado no Github, faça todo desafio na branch master e não se esqueça de preencher o arquivo pull-request.txt. Tão logo termine seu desenvolvimento, adicione como colaborador o usuário ic-validator no seu repositório e o deixe disponível por pelo menos 30 dias. Não adicione o ic-validator antes do término do desenvolvimento.
- O código precisa rodar preferencialmente como container Docker.
- Deverá ter as chamadas na API criadas no PostMan e disponibilizadas no repositório

Para executar seu código, deve ser preciso apenas rodar os seguintes comandos:
- git clone $seu-fork
- cd $seu-fork
- comando para instalar dependências
- comando para executar a aplicação

A API pode ser escrita com ou sem a ajuda de frameworks
Se optar por usar um framework que resulte em boilerplate code, assinale no README qual pedaço de código foi escrito por você. Quanto mais código feito por você, mais conteúdo teremos para avaliar.

## Critério de avaliação
- Organização do código
- Assertividade
- Legibilidade do código
- Cobertura de testes
- Histórico de commits
- A API é intuitiva?
- Clareza: O README explica de forma resumida qual é o problema e como pode rodar a aplicação?
- Escolhas técnicas: A escolha das bibliotecas, banco de dados, arquitetura, etc, é a melhor escolha para a aplicação?
- UX: A interface é de fácil uso e auto-explicativa? (Bonus point)

Boa sorte ;)
