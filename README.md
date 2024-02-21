## Shopware 6 Update Locally
- Setup latest version of a local dev environment with database
- bin/console system:update:prepare
- change package versions in composer.json
    core, storefront, administration
- composer update
- check if every package is "updateable" and compatible
- bin/console system:update:finish
- composer recipes:update
    execute suggested command for each package
- sudo rm -r vendor
- composer install
- bin/build-js.sh
- testing storefront, administration, apps, plugins, custom fields and cronjobs
- git push update feature

## Shopware 6 Update Production
- backup to save configuration files..
- merge update feature
