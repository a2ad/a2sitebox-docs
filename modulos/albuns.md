Módulo de Álbuns (Galeria)
==========================

Esse módulo tem como objetivo possibilitar ao usuário a criação de galerias de imagens para posterior visualização dentro do módulo de postagens por exemplo.

**Funcionalidades**

* Inclusão de galeria
* Edição de galeria
* Ordenação de fotos da galeria
* Inclusão de mídia (diretamente da página de criação/edição da galeria)

**Estrutura do módulo**

```
AlbunsBundle/
├── A2SiteboxAlbunsBundle.php
├── Controller
│   └── AlbunsController.php
├── DependencyInjection
│   ├── A2SiteboxAlbunsExtension.php
│   └── Configuration.php
├── Entity
│   ├── Albuns.php
│   └── AlbunsRepository.php
├── Filter
│   └── AlbunsFilterType.php
├── Form
│   └── AlbunsType.php
├── Resources
│   ├── config
│   │   └── services.xml
│   └── views
│       ├── Albuns
│       │   ├── edit.html.twig
│       │   ├── index.html.twig
│       │   ├── new.html.twig
│       │   ├── new_in_posts.html.twig
│       │   ├── tabela.html.twig
│       │   └── tabela_icon.html.twig
│       ├── Box
│       │   ├── filtro.html.twig
│       │   └── publicar.html.twig
│       ├── Form
│       │   ├── delete.html.twig
│       │   └── fields.html.twig
│       ├── List
│       │   ├── album_update.html.twig
│       │   └── list.html.twig
│       └── Modal
│           └── new.html.twig
└── Tests
    └── Controller
        └── DefaultControllerTest.php
```

**Diagrama de classe**

O diagrama abaixo representa a classe Albuns.php

![Albuns Class Diagram](https://github.com/a2comunicacao/a2sitebox-docs/blob/2.0/modulos/diagramas/albuns.png "Albuns Class Diagram")
