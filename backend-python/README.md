![portaldetodos](https://avatars0.githubusercontent.com/u/56608703?s=400&u=ae31a7a07d28895589b42ed0fcfc102c3d5bccff&v=4)

Desafio técnico `Python`
========================

Alguns requisitos
-----------------
  - Deixe o código em inglês;
  - Use Git;
  - Procure fazer `micro commits` que são muitos commits com menos código isso nos ajuda a compreender a sua lógica;
  - Nos pergunte sobre qualquer dúvida que venha a surgir durante o desenvolvimento;
  - Documente detalhadamente quaisquer referencias/ferramentas que vc pesquisar;
  - Crie um repositório público e nos passe o link para acompanharmos o desenvolvimento;
  - Faça testes;

Problema
--------

A `CREDTODOS LTDA` está lançando um sistema inovador de cadastros de clientes e precisa garantir toda a qualidade e padronização dos dados.
E esse sistema será uma `API` simples de cadastro de clientes, e o sistema irá receber no cadastro:
```shell
NOME
EMAIL
TELEFONE
CEP
NUMERO
COMPLEMENTO
CPF
```

Como não é um cadastro qualquer, esses dados precisam passar por uma validação criteriosa e específica:

- EMAIL
  - Se não existe na base
  - Pode utilizar via regex, lib ou até api https://verifalia.com/email-verification-api

- TELEFONE
  - Se é um telefone válido
  - Existem libs de validação de telefone, por exemplo, https://pypi.org/project/phonenumbers/

- CEP
  - Verificar se o cep realmente existe
  - Complementar os dados, utilize algum serviço externo, por exemplo, https://viacep.com.br/ws/11030904/json/

- NUMERO e COMPLEMENTO
  - não são obrigatórios, mais o número deve ser válido

- CPF
  - verificar se o valor é válido

A api deve conter basicamente as urls (sugestão):
```shell
  GET  /api/v1/customers - listar os clientes
  GET  /api/v1/customers/`<key>` - detalhe do cliente
  POST /api/v1/customers - cadastrar um novo cliente
```

O acesso à api deve ser aberto ao mundo, porém deve possuir autenticação e autorização.

Você está livre para definir a melhor arquitetura e tecnologias para solucionar este desafio, todos os itens descritos nos campos são `sugestões`, mas não se esqueça de contar sua motivação no arquivo README que deve acompanhar sua solução, junto com os detalhes de como executar seu programa. Documentação e testes serão avaliados também =).

Nós solicitamos que você trabalhe no desenvolvimento desse sistema sozinho e não divulgue a solução desse problema pela internet.

Boa sorte,
PagTodos e CredTodos!

![Luck](https://media.tenor.com/images/e026ce9d75219c8d82277ddf0558ee2b/tenor.gif)
