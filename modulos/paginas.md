Módulo de Páginas
=================

Esse módulo tem como objetivo possibilitar ao usuário a criação de páginas, selecionado um template e fazendo a edição do conteúdo da página através de blocos.

**Funcionalidades**

* Inclusão de página
* Edição de página
* Exclusão de página

**Estrutura do módulo**

```
PaginasBundle/
├── A2SiteboxPaginasBundle.php
├── Controller
│   └── PaginasController.php
├── DependencyInjection
│   ├── A2SiteboxPaginasExtension.php
│   └── Configuration.php
├── Entity
│   ├── Paginas.php
│   ├── PaginasRepository.php
│   └── PaginasTemplates.php
├── Event
│   ├── PaginaEvents.php
│   └── PaginaUpdateEvent.php
├── EventListener
│   ├── MenuUpdateListener.php
│   └── NivelUpdateListener.php
├── Filter
│   └── PaginasFilterType.php
├── Form
│   ├── EventListener
│   │   └── AddStatusFieldSubscriber.php
│   └── PaginasType.php
├── Resources
│   ├── config
│   │   ├── services.xml
│   │   └── validation.yml
│   ├── doc
│   │   └── index.rst
│   └── views
│       ├── Bar
│       │   └── edit.html.twig
│       ├── Box
│       │   ├── filtro.html.twig
│       │   └── publicar.html.twig
│       ├── Form
│       │   ├── configuracoes.html.twig
│       │   ├── delete.html.twig
│       │   ├── fields.html.twig
│       │   └── new.html.twig
│       ├── Modal
│       │   └── edit.html.twig
│       └── Paginas
│           ├── index.html.twig
│           ├── new.html.twig
│           ├── scripts.html.twig
│           ├── tabela.html.twig
│           └── tbody.html.twig
├── Tests
│   └── Controller
│       └── PaginasControllerTest.php
└── Twig
    └── PageUrlGeneratorExtension.php

```

**Diagrama de classe**

O diagrama abaixo representa a classe Páginas.php

![Paginas Class Diagram](https://github.com/a2comunicacao/a2sitebox-docs/blob/2.0/modulos/diagramas/paginas.png "Paginas Class Diagram")
