This is default sublime configuration used in Suitmedia

# Requirement

1. PHP 5
1. [Composer](https://getcomposer.org)

# Installation

For Windows

1. Remove or backup `Data` Directory in sublime directory. Here are default sublime directory `<Installation Dir>/Data`
1. In Sublime Configuration directory, clone this repo to `Data`
1. Move to `<Installation Dir>/Data`
1. Run `composer install`
1. Install [PHPMD](http://pear.phpmd.org/) and  PHP_CodeSniffer via pear. Install pear from [here](https://pear.php.net/manual/en/installation.getting.php)
1. Register Suitmedia Code Standards, `phpcs --config-set installed_paths <Installation Dir>\Data\vendor\suitmedia\php-code-standards`.
If `permission denied` occured follow [this solution](http://stackoverflow.com/questions/10397203/php-pear-on-windows-tries-to-open-c-windows-pear-ini-for-writing-even-though-t)
1. Edit phpcs package configuration file `Packages\User\phpcs.sublime-settings`, or via Sublime `Preferences > Package Settings > PHP Code Sniffer > Settings - Users`
```
    "phpcs_executable_path": "<path_to_php_bin>/phpcs.bat",
    "phpmd_executable_path": "<path_to_php_bin>/phpmd.bat",
```

For Linux

1. Remove or backup sublime directory in `$HOME/.config/sublime-text-3`.
1. Clone this repo to `$HOME/.config/sublime-text-3/`
1. Move to `$HOME/.config/sublime-text-3/`
1. Run `composer install`
1. Register Suitmedia Code Standards, `./vendor/bin/phpcs --config-set installed_paths $HOME/.config/sublime-text-3/vendor/suitmedia/php-code-standards`
1. Edit phpcs package configuration file `Packages/User/phpcs.sublime-settings`, or via Sublime `Preferences > Package Settings > PHP Code Sniffer > Settings - Users`
```
    "phpcs_executable_path": "$HOME/.config/sublime-text-3/vendor/bin/phpcs",
    "phpmd_executable_path": "$HOME/.config/sublime-text-3/vendor/bin/phpmd",
```

# Package List

- [All Autocomplete](https://github.com/alienhard/SublimeAllAutocomplete)
- [Emmet](https://github.com/emmetio/emmet)
- [Git](https://github.com/kemayo/sublime-text-git)
- [GitGutter](https://github.com/jisaacks/GitGutter)
- [Laravel Blade Highlighter](https://github.com/Medalink/laravel-blade)
- [PHP CS](https://github.com/benmatselby/sublime-phpcs)
- [PHP Companion](https://github.com/erichard/SublimePHPCompanion)


