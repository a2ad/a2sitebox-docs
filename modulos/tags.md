Módulo de Tags
==============

Esse módulo tem como objetivo possibilitar ao usuário a inserir tags para posterior relacionar dentro do módulo de postagens.

**Funcionalidades**

* Inclusão de tags
* Edição de tags
* Exclusão de tags

**Estrutura do módulo**

```
TagsBundle/
├── A2SiteboxTagsBundle.php
├── Controller
│   └── TagsController.php
├── DependencyInjection
│   ├── A2SiteboxTagsExtension.php
│   └── Configuration.php
├── Entity
│   ├── Tags.php
│   └── TagsRepository.php
├── Filter
│   └── TagsFilterType.php
├── Form
│   └── TagsType.php
├── Resources
│   ├── config
│   │   └── services.xml
│   └── views
│       ├── Tags
│       │   ├── edit.html.twig
│       │   ├── index.html.twig
│       │   ├── new.html.twig
│       │   ├── tabela.html.twig
│       ├── Box
│       │   ├── filtro.html.twig
│       │   └── publicar.html.twig
│       ├── Form
│       │   ├── delete.html.twig
│       │   └── fields.html.twig
└── Tests
    └── Controller
        └── DefaultControllerTest.php
           
        
```

**Diagrama de classe**

O diagrama abaixo representa a classe Tags.php

![Tags Class Diagram](https://github.com/a2comunicacao/a2sitebox-docs/blob/2.0/modulos/diagramas/tags.png "Tags Class Diagram")

