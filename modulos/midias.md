Módulo de Mídias
==============

Esse módulo tem como objetivo possibilitar ao usuário a inserir mídias para posterior relacionar dentro do módulo de postagens.

**Funcionalidades**

* Inclusão de midia
* Edição de midia
* Exclusão de midia

**Estrutura do módulo**

```
MidiasBundle/
├── A2SiteboxMidiasBundle.php
├── Controller
│   └── MidiaController.php
├── DependencyInjection
│   ├── A2SiteboxMidiasExtension.php
│   └── Configuration.php
├── Entity
│   ├── Audio.php
│   ├── Documento.php
│   ├── Imagem.php
│   ├── MidiaInfo.php
│   ├── Midia.php
│   ├── MidiaRepository.php
│   ├── TipoMidia.php
│   ├── UploadedMidiaManager.php
│   └── Video.php
├── Filter
│   └── MidiaFilterType.php
├── Form
│   ├── CropType.php
│   ├── EventListener
│   │   └── AddFileMidiaField.php
│   ├── MidiaType.php
│   └── YoutubeType.php
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
│       ├── Form
│       │   ├── delete.html.twig
│       │   ├── edit_fields.html.twig
│       │   ├── editMidiaList.html.twig
│       │   └── fields.html.twig
│       ├── List
│       │   ├── list.html.twig
│       │   └── midia_update.html.twig
│       ├── Midia
│       │   ├── crop.html.twig
│       │   ├── edit.html.twig
│       │   ├── index.html.twig
│       │   ├── new.html.twig
│       │   ├── tabela.html.twig
│       │   └── tabela_icon.html.twig
│       ├── Modal
│       │   └── new.html.twig
│       └── Plugin
│           ├── image.html.twig
│           └── images.html.twig
└── Tests
    └── Controller
        └── MidiaControllerTest.php
           
        
```

**Diagrama de classe**

O diagrama abaixo representa a classe Midia.php

![Midias Class Diagram](https://github.com/a2comunicacao/a2sitebox-docs/blob/2.0/modulos/diagramas/midias.png "Midias Class Diagram")

