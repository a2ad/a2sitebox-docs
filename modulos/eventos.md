Módulo de Eventos
=================

Esse módulo tem como objetivo possibilitar ao usuário a inserir um evento sendo possível relacionar com o módulo de mídias, categorias e endereços.

**Funcionalidades**

* Inclusão de evento
* Edição de evento
* Exclusão de evento

**Estrutura do módulo**

```
EventosBundle/
├── A2SiteboxEventosBundle.php
├── Controller
│   └── EventoController.php
├── DependencyInjection
│   ├── A2SiteboxEventosExtension.php
│   └── Configuration.php
├── Entity
│   ├── Evento.php
│   └── EventoRepository.php
├── Filter
│   └── EventoFilterType.php
├── Form
│   └── EventoType.php
├── Resources
│   ├── config
│   │   ├── services.xml
│   │   └── validation.yml
│   ├── doc
│   │   └── index.rst
│   └── views
│       ├── Box
│       │   ├── filtro.html.twig
│       │   └── publicar.html.twig
│       ├── Evento
│       │   ├── edit.html.twig
│       │   ├── index.html.twig
│       │   ├── new.html.twig
│       │   └── tabela.html.twig
│       └── Form
│           └── fields.html.twig
└── Tests
    └── Controller
        └── EventoControllerTest.php
        
```

**Diagrama de classe**

O diagrama abaixo representa a classe Evento.php

![Eventos Class Diagram](https://github.com/a2comunicacao/a2sitebox-docs/blob/2.0/modulos/diagramas/eventos.png "Eventos Class Diagram")

