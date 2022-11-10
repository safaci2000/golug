# What is This?

The purpose of this repo is to show case a really basic REST Crud service.

# Why are you using <package>?

Cause I want to.  They're all opinionated choices and not the best or worst but should work for the use case I'm presenting. 

Logging:

[Logrus](https://github.com/sirupsen/logrus) I like it since it's simple to setup and requires basically no configuration.

Database:

[PostgresSQL](https://www.postgresql.org/) Same, I'm more familiar with it than MySQL. It's more SQL standard compliant and more feature rich.  Also, just simply cause I want to. 

[Chi](https://github.com/go-chi/chi) GoLang router.  I've been meaning to look at this for a while so this is a good excuse.  Therefore, I'm embracing my inner Chi.

[Viper](https://github.com/spf13/viper) At this point it feels silly not to use this. It supports, YAML, JSON, ini, hcl, toml, javaproperties, ENV overrides.

More DataBase Opinions: 

[DBMate](https://github.com/amacneil/dbmate) Schema management, requires more writing of raw sql, but I'm a bit fan of Schema first design, so there we go.

[SQLBoiler](github.com/volatiletech/sqlboiler/) Partly I like the SQL and wanted to play with this approach more.  DB first design. An alternative that I've heard good things about haven't explored yet is [SQLC](https://github.com/kyleconroy/sqlc)

## Install Packages

```sh
## DBMate
brew install dbmate # for mac
##Linux
sudo curl -fsSL -o /usr/local/bin/dbmate https://github.com/amacneil/dbmate/releases/latest/download/dbmate-linux-amd64
sudo chmod +x /usr/local/bin/dbmate
##Needed for code generation
go install github.com/volatiletech/sqlboiler/v4@latest
go install github.com/volatiletech/sqlboiler/v4/drivers/sqlboiler-psql@latest
```