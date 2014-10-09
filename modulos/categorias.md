Módulo de Categorias
====================

Esse módulo tem como objetivo possibilitar ao usuário a inserir categorias, relacionar a uma categoria pai e definir os módulos associados (Postagens, Midias, Eventos e Endereços).

**Funcionalidades**

* Inclusão de categoria
* Edição de categoria
* Exclusão de categoria

**Estrutura do módulo**

```
CategoriasBundle/
├── A2SiteboxCategoriasBundle.php
├── Controller
│   └── CategoriaController.php
├── DependencyInjection
│   ├── A2SiteboxCategoriasExtension.php
│   └── Configuration.php
├── Entity
│   ├── Categoria.php
│   ├── CategoriaRepository.php
│   └── CategoriaTipo.php
├── Filter
│   └── CategoriaFilterType.php
├── Form
│   └── CategoriaType.php
├── Resources
│   ├── config
│   │   ├── services.xml
│   │   └── validation.yml
│   ├── doc
│   │   └── index.rst
│   └── views
│       ├── Box
│       │   ├── add_categoria.html.twig
│       │   ├── categorias.html.twig
│       │   ├── filtro.html.twig
│       │   └── publicar.html.twig
│       ├── Categoria
│       │   ├── edit.html.twig
│       │   ├── index.html.twig
│       │   ├── new.html.twig
│       │   ├── tabela.html.twig
│       │   └── tbody.html.twig
│       └── Form
│           └── fields.html.twig
└── Tests
    └── Controller
        └── CategoriaControllerTest.php
        
```

**Diagrama de classe**

O diagrama abaixo representa a classe Categoria.php

![Categorias Class Diagram](https://github.com/a2comunicacao/a2sitebox-docs/blob/2.0/modulos/diagramas/categorias.png "Categorias Class Diagram")

