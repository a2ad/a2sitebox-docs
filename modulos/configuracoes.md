Módulo de Configurações
=======================

Esse módulo tem como objetivo possibilitar ao usuário a configurar o website.

**Funcionalidades**

* Configuração de nome do website
* Configuração de URL do website
* Configuração de email de contato

**Estrutura do módulo**

```
ConfiguracoesBundle/
├── A2SiteboxConfiguracoesBundle.php
├── Controller
│   └── ConfiguracoesController.php
├── DependencyInjection
│   ├── A2SiteboxConfiguracoesExtension.php
│   └── Configuration.php
├── Entity
│   ├── Configuracoes.php
│   └── ConfiguracoesRepository.php
├── EventListener
│   └── SiteConfigurationListener.php
├── Form
│   └── ConfiguracoesType.php
└── Resources
    ├── config
    │   ├── services.xml
    │   └── validation.yml
    ├── doc
    │   └── index.rst
    └── views
        ├── Box
        │   └── publicar.html.twig
        ├── Configuracoes
        │   ├── edit.html.twig
        │   ├── index.html.twig
        │   ├── new.html.twig
        │   └── site_confs.html.twig
        └── Form
            └── fields.html.twig
        
```

**Diagrama de classe**

O diagrama abaixo representa a classe Configuracoes.php

![Configuracoes Class Diagram](https://github.com/a2comunicacao/a2sitebox-docs/blob/2.0/modulos/diagramas/configuracoes.png "Configuracoes Class Diagram")

