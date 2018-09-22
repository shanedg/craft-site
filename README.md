# craft-site

CraftCMS 3 for work and for pleasure

## installation

### mac os
#### composer w/ homebrew:
1. run `brew install composer`
2. run `composer install`

#### using MAMP w/ homebrew cask and postgres via Postgres.app:
1. `brew cask install mamp`
2. 'MAMP' > Preferences > Web Server > set document root to `.../craft-site/web/`
    * apache works for our purposes out-of-the-box
    * **TODO:** nginx needs more config
3. download and install Postgres app from https://postgresapp.com/
    * note Postgres.app default settings [here](https://postgresapp.com/#installing-postgresapp)
    * **OPTIONAL:** include provided [cli tools](https://postgresapp.com/documentation/cli-tools.html) in your PATH, e.g. `PATH=$PATH:/Applications/Postgres.app/Contents/Versions/latest/bin`

#### db [security key](https://craftcms.stackexchange.com/a/23230/8831), other environment settings:
Populates values in your `.env` file, excluded from version control
1. generate a security key for your db, `./craft setup/security-key`
2. run craft setup, `./craft setup` to populate db settings (postgres must be running)

## run

**TODO:** more detail
1. but basically start mamp servers, start postgres
