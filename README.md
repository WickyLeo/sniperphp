# PHP Code Standrd Check 

## What's this?
PHP Code pre-commit hook to git or gitlab,checkout your code style PSR Compliance.
Base on *PHP Sniffer*, and use `php -l` to checkout basic syntax.
You can change rule set if you want to change PSR Compliance,modify `ruleset.xml` and Specified your rule. 

## How to use?
Add the following paragraph in composer.json,
```
{
    "require-dev": {
        "sniperphp/code_check":"dev-master"
    },
    "repositories": [
        {
            "type": "git",
            "url": "https://github.com/WickyLeo/sniperphp"
        }
    ],
    "scripts": {
        "post-install-cmd": [
            "sh ./vendor/sniperphp/code_check/setup_hooks.sh"
        ],
        "post-update-cmd": [
            "sh ./vendor/sniperphp/code_check/setup_hooks.sh"
        ]
    }
}
```
and in your project root path, execute
```
composer install or composer update
```

