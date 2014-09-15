Módulo de Comentários
=====================

Esse módulo tem como objetivo possibilitar ao usuário a moderar os comentários relacionados a uma página ou postagem.

**Funcionalidades**

* Aprovar comentário
* Reprovar comentário

**Estrutura do módulo**

```
ComentariosBundle/
├── A2SiteboxComentariosBundle.php
├── Controller
│   └── ComentariosController.php
├── DependencyInjection
│   ├── A2SiteboxComentariosExtension.php
│   └── Configuration.php
├── Entity
│   ├── Comentarios.php
│   └── ComentariosRepository.php
├── Filter
│   └── ComentariosFilterType.php
├── Form
│   └── ComentariosType.php
├── Resources
│   ├── config
│   │   └── services.xml
│   └── views
│       ├── Comentarios
│       │   ├── index.html.twig
│       │   ├── moderar.html.twig
│       │   ├── tabela_moderar.html.twig
│       │   ├── tabela.html.twig
│       ├── Box
│       │   ├── filtro_moderar.html.twig
│       │   └── filtro.html.twig
└── Tests
    └── Controller
        └── DefaultControllerTest.php
           
        
```

**Diagrama de classe**

O diagrama abaixo representa a classe Comentarios.php

![Comentarios Class Diagram](https://github.com/a2comunicacao/a2sitebox-docs/blob/2.0/modulos/diagramas/comentarios.png "Comentarios Class Diagram")

