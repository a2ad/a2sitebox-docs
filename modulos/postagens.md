Módulo de Postagens
===================

Esse módulo tem como objetivo possibilitar ao usuário a criação de postagens, integrando com os módulos de Mídias, Albuns, Categorias, Tags e a possibilidade de relacionar uma Postagem.

**Funcionalidades**

* Inclusão de postagem
* Edição de postagem
* Exclusão de postagem

**Estrutura do módulo**

```
PostagensBundle/
├── A2SiteboxPostagensBundle.php
├── Controller
│   └── PostagensController.php
├── DependencyInjection
│   ├── A2SiteboxPostagensExtension.php
│   └── Configuration.php
├── Entity
│   ├── Postagens.php
│   └── PostagensRepository.php
├── Filter
│   └── PostagensFilterType.php
├── Form
│   └── PostagensType.php
├── Resources
│   ├── config
│   │   ├── services.xml
│   │   └── validation.yml
│   └── views
│       ├── Box
│       │   ├── album.html.twig
│       │   ├── filtro.html.twig
│       │   ├── publicar.html.twig
│       │   ├── relacionar_postagens.html.twig
│       │   └── tags.html.twig
│       ├── Form
│       │   ├── delete.html.twig
│       │   └── fields.html.twig
│       └── Postagens
│           ├── edit.html.twig
│           ├── index.html.twig
│           ├── new.html.twig
│           └── tabela.html.twig
├── Tests
│   └── Controller
│       └── PostagensControllerTest.php
└── Twig
    ├── DateDifferenceExtension.php
    └── DateIntlExtension.php
```

**Diagrama de classe**

O diagrama abaixo representa a classe Postagens.php

![Postagens Class Diagram](https://github.com/a2comunicacao/a2sitebox-docs/blob/2.0/modulos/diagramas/postagens.png "Postagens Class Diagram")
