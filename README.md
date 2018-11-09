# craft-site

CraftCMS 3 for work and for pleasure

## installation

### mac os
#### composer w/ homebrew:
1. run `brew install composer`
2. run `composer install`

#### using MAMP and postgres via homebrew:
1. `brew cask install mamp`
2. 'MAMP' > Preferences > Web Server > set document root to `.../craft-site/web/`
    * apache works for our purposes out-of-the-box
    * **TODO:** nginx needs more config
3. `brew install postgres`

#### db [security key](https://craftcms.stackexchange.com/a/23230/8831), other environment settings:
Populates values in your `.env` file, excluded from version control
1. generate a security key for your db, `./craft setup/security-key`
2. run craft setup, `./craft setup` to populate db settings (postgres must be running)

## run

**TODO:** more detail
1. `brew services start postgresql`
2. start mamp servers
