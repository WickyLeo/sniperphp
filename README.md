# PHP Code Standrd Check 

## What's this?
PHP Code pre-commit to git or gitlab,checkout your code style PSR Compliance.

## How to use?
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
