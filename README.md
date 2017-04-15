# Magento coding standard
This is the default coding standard being used by Magento 2 core team.

# Usage

I assume all of developers using PhpStorm or smiliar IDE to coding right now
in Balance Internet. If you don't, you can contact me privately to get a key (legally)
of it.

## MacOS

### Prerequisites

[__Homebrew__](https://brew.sh) __installed__

Q: Why Homebrew?
A-Short version: Why not?
A-Long version: It's apt-get/yum tool dedicated for MacOS

### Installation

* `brew tap homebrew/homebrew-php`
* `brew update`
* `brew install php56` (php53 php54 php55 php70, your choices)
* `brew install php-code-sniffer` (bonus `brew install phpmd`)

### Set it up

* Clone this repo to wherever you want
* Symlink it to `/usr/local/etc/php-code-sniffer/Standards`

E.g:
```
$ git clone https://github.com/balanceinternet/coding-standard BalanceInternet_phpcs
$ ln -s BalanceInternet_phpcs/Magento /usr/local/etc/php-code-sniffer/Standards/BalanceM2
```

Q: Why symlink?
A: Homebrew

#### Integrate with PhpStorm

* Navigate to __Preferences__ > __PHP__ > __Code Sniffer__
* Set path to output of `which phpcs` and hit 'validate'
* Navigate to __Preferences__ > __Inspections__ > __PHP__ > __PHP Code Sniffer__ validation and tick to enable
* Refresh 'Coding Standards' dropdown and select your preferred options (_BalanceM2_ obviously)