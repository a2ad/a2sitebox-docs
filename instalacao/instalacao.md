Instalação
----------------

Antes de iniciar a instalação certifique-se de que possui os requisitos abaixo:

* PHP 5.4+
* Extensões INTL, JSON, mysql e ctype habilitadas
* Banco de dados MySql
* Servidor Apache com mod_rewrite habilitado

Passo a passo
-------------

Baixe a última release relacionada a versão 2.0.* no repositório do [A2siteBox](https://github.com/a2comunicacao/A2SiteBox/releases).

Realize a extração dos arquivos na pasta do novo projeto você deve ter uma estrutura como essa:

```
├── app/
├── bin/
├── composer.json
├── composer.lock
├── composer.phar
├── LICENSE
├── README.md
├── src/
├── UPGRADE.md
├── vendor/ --------------> Essa pasta será criada após o próximo passo
└── web/    --------------> O DocumentRoot do Apache deve apontar para essa pasta
```

Crie os diretórios de cache `app/cache/` e também `web/cache/` com permissão de leitura, escrita e execução (777).

Abra o terminal na pasta do projeto e digite o comando do composer para instalar as dependências:

`php composer.phar install`
    
Obs: Esse processo pode demorar

Enquanto isso vá até a pasta `app/config`, crie um arquivo chamado `parameters.ini` e coloque o conteúdo abaixo substituindo o nome do banco de dados (database_name), o nome do usuário do banco (database_user) e a senha do banco de dados (database_password) pelos dados de sua máquina/servidor:

```
[parameters]
  database_driver="pdo_mysql"
  database_host="localhost"
  database_port=""
  database_name="dbname"
  database_user="dbuser"
  database_password="dbpass"
  support_email="suporte@a2sitebox.com.br"
  contato_email="info@a2comunicacao.com.br"
  trabalhe_email="vagas@a2comunicacao.com.br"
  proposta_email="atendimento@a2comunicacao.com.br"
  mailer_transport="gmail"
  mailer_host="localhost"
  mailer_user="user@gmail.com"
  mailer_password="gmailuserpass"
  locale="pt_BR"
  secret="8a0afc1dcf295ee403445c5da6902ba52fdbabeb"
```

Dentro da pasta `app/config/schema/` está o banco de dados da versão que está utilizando ( ex. a2sitebox_aquario_v2.0.0.sql ), importe esse arquivo no seu banco de dados e ele irá criar as tabelas e inserir os dados necessários para a aplicação funcionar corretamente.

Para acessar o A2siteBox supondo que você criou um ambiente chamado `a2sitebox.local` basta acessar:

`http://a2sitebox.local/a2sitebox/login`

Utilize as credenciais abaixo para acessar:

```
  E-mail: admin@a2comunicacao.com.br
  Senha: a2siteboxaquarius
```

Pronto!
