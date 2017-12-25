# PHP Code Standrd Check 

## What's this?
PHP Code pre-commit to git or gitlab,checkout your code style PSR Compliance.

## How to use?
```
{
    "require-dev": {
        "selfiecity/code_standard":"dev-master"
    },
    "repositories": [
        {
            "type": "git",
            "url": "https://github.com/WickyLeo/codeCheck.git"
        }
    ],
    "scripts": {
        "post-install-cmd": [
            "sh ./vendor/codecheck/code_standard/setup_hooks.sh"
        ],
        "post-update-cmd": [
            "sh ./vendor/codecheck/code_standard/setup_hooks.sh"
        ]
    }
}
```
