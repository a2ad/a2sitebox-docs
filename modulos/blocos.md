Módulo de Blocos
================

Esse módulo tem como objetivo compor uma página do A2siteBox, portanto é um módulo abstrato. Os módulos possuem um formulário para edição no administrador e são renderizados em html.

**Funcionalidades**

* Inclusão de blocos em uma página
* Edição de blocos de uma página

**Blocos disponíveis**

* Categoria - Lista postagens relacionadas à uma categoria
 * Template: categoria.html.twig
 * Formulário: CategoriaType.php

* Endereço - Gera uma imagem do Google Maps (estática) do endereço selecionado
 * Template: endereco.html.twig
 * Formulário: EnderecoType.php

* File (Arquivo) - Cria um link com o arquivo para download
 * Template: file.html.twig
 * Formulário: FileType.php

* Imagem - Gera uma tag img da imagem selecionada
 * Template: imagem_destaque.html.twig
 * Formulário: ImagemType.php

* News (Notícias) - Gera um bloco com link para a postagem, titulo e o texto inseridos
 * Template: news.html.twig
 * Formulário: NewsType.php

* RichText - Bloco de texto com editor tinyMCE, renderiza o html inserido no editor
 * Template: rich_text.html.twig
 * Formulário: RichTextType.php

Obs. Os templates ficam no diretório `Resources/views/Widget/`

**Estrutura do módulo**

```
BlocosBundle/
├── A2SiteboxBlocosBundle.php
├── Controller
│   └── BlocoController.php
├── DependencyInjection
│   ├── A2SiteboxBlocosExtension.php
│   └── Configuration.php
├── Entity
│   ├── BlocoManager.php
│   ├── Bloco.php
│   ├── BlocoRepository.php
│   ├── Categoria.php
│   ├── Endereco.php
│   ├── File.php
│   ├── Imagem.php
│   ├── News.php
│   └── RichText.php
├── Form
│   ├── BlocoType.php
│   ├── CategoriaType.php
│   ├── EnderecoType.php
│   ├── EventListener
│   │   ├── PopulateFieldsSubscriber.php
│   │   └── RichTextFieldSubscriber.php
│   ├── FileType.php
│   ├── ImagemType.php
│   ├── NewsType.php
│   └── RichTextType.php
├── Resources
│   ├── config
│   │   └── services.xml
│   ├── doc
│   │   └── index.rst
│   └── views
│       ├── Bloco
│       │   └── gera_form.html.twig
│       ├── Form
│       │   └── form_layout.html.twig
│       └── Widget
│           ├── categoria.html.twig
│           ├── contentloader.html.twig
│           ├── default.html.twig
│           ├── endereco.html.twig
│           ├── file.html.twig
│           ├── imagem_destaque.html.twig
│           ├── news.html.twig
│           └── rich_text.html.twig
└── Tests
    └── Controller
        └── BlocoControllerTest.php

```

**Diagrama de classe**

O diagrama de classes abaixo representa as entidades desse módulo

![Blocos Class Diagram](https://github.com/a2comunicacao/a2sitebox-docs/blob/2.0/modulos/diagramas/blocos.png "Blocos Class Diagram")
