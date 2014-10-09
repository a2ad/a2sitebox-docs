Módulo de Endereços
===================

Esse módulo tem como objetivo possibilitar ao usuário a inserir endereços sendo possível relacionar com o módulo de categorias.

**Funcionalidades**

* Inclusão de endereço
* Edição de endereço
* Exclusão de endereço

**Estrutura do módulo**

```
EnderecosBundle/
├── A2SiteboxEnderecosBundle.php
├── Controller
│   └── EnderecoController.php
├── DependencyInjection
│   ├── A2SiteboxEnderecosExtension.php
│   └── Configuration.php
├── Entity
│   ├── Endereco.php
│   └── EnderecoRepository.php
├── Filter
│   └── EnderecoFilterType.php
├── Form
│   └── EnderecoType.php
├── Resources
│   ├── config
│   │   ├── services.xml
│   │   └── validation.yml
│   ├── doc
│   │   └── index.rst
│   ├── translations
│   │   └── messages.fr.xlf
│   └── views
│       ├── Box
│       │   ├── filtro.html.twig
│       │   └── publicar.html.twig
│       ├── Endereco
│       │   ├── edit.html.twig
│       │   ├── index.html.twig
│       │   ├── new.html.twig
│       │   └── tabela.html.twig
│       ├── Form
│       │   └── fields.html.twig
│       └── Modal
│           └── new.html.twig
└── Tests
    └── Controller
        └── EnderecoControllerTest.php
        
```

**Diagrama de classe**

O diagrama abaixo representa a classe Endereco.php

![Enderecos Class Diagram](https://github.com/a2comunicacao/a2sitebox-docs/blob/2.0/modulos/diagramas/endereco.png "Enderecos Class Diagram")

