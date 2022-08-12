# vs-theme

### vscode setting.json:
```
{
    "workbench.startupEditor": "none",
    "php.validate.executablePath": "D:/xampp/php/php.exe",
    "editor.minimap.enabled": false,
    "editor.wordWrap": "on",
    "workbench.colorTheme": "VS Theme",
    "workbench.sideBar.location": "right",
    "git.ignoreMissingGitWarning": true,
    "explorer.autoReveal": false,
    "editor.fontFamily": "'Cascadia Code', Consolas, 'Courier New', monospace",
    "editor.fontWeight": "400",
    "editor.fontLigatures": true,
    "editor.lineHeight": 1.4,
    "editor.letterSpacing": 0.3,
}
```

### vscode php snippets:
```
{
	"PHP tags": {
        "prefix": "php",
        "body": [
            "<?php $0?>"
        ],
        "description": "PHP open tag"
    },
    "PHP open tag": {
        "prefix": "po",
        "body": [
            "<?php"
        ],
        "description": "PHP open tag"
    },
    "PHP close tag": {
        "prefix": "pc",
        "body": [
            "?>"
        ],
        "description": "PHP close tag"
    },
    "PHP echo short tag": {
        "prefix": "peco",
        "body": [
            "<?= \\$${1:variable} ?>"
        ],
        "description": "PHP echo short tag"
    },
	"PHP reverse tag": {
        "prefix": "prve",
        "body": [
            "?> $0 <?php"
        ],
        "description": "PHP echo short tag"
    },    
	"PHP array print":{
		"prefix": "prna",
		"body": [
			"echo '<pre>' , print_r($array, true) , '</pre>'"
		],
		"description": "PHP print array"
	},
	"Exit ABSPATH":{
		"prefix": "exap",
		"body": [
			"if ( !defined('ABSPATH') ) { \n\texit; // Exit if accessed directly \n}"
		],
		"description": "Exit if abspath undefined"
	},
	
	"<?php If ... endif": {
        "prefix": "pifen",
        "body": [
            "<?php if (${1:condition}): ?>",
            "\t${0:<!-- coding here -->}",
            "<?php endif; ?>"
        ],
        "description": "If endif block inside HTML"
    },
    "<?php If ... else ... endif": {
        "prefix": "pifelen",
        "body": [
            "<?php if (${1:condition}): ?>",
            "\t${2:<!-- coding here -->}",
            "<?php else: ?>",
            "\t${0:<!-- coding here -->}",
            "<?php endif ?>;"
        ],
        "description": "If else endif block"
    },
    "<?php If ... elseif ... else ... endif": {
        "prefix": "pifelifen",
        "body": [
            "<?php if (${1:condition}): ?>",
            "\t${2:<!-- coding here -->}",
            "<?php elseif (${3:condition}): ?>",
            "\t${4:<!-- coding here -->}",
            "<?php else: ?>",
            "\t${0:<!-- coding here -->}",
            "<?php endif; ?>"
        ],
        "description": "If elseif else endif block"
    },
    "<?php Ternary operator": {
        "prefix": "ptern",
        "body": [
            "<?php ${1:condition} ? ${2:if_true} : ${3:if_false}; ?>"
        ],
        "description": "Ternary statement"
    }
}
```
### vscode keybindding.json
```
// Place your key bindings in this file to override the defaults
[
    {
        "key": "ctrl+n",
        "command": "explorer.newFile",
        "when": "explorerViewletFocus"
    },
    {
        "key": "ctrl+shift+n",
        "command": "explorer.newFolder",
        "when": "explorerViewletFocus"
    },
    {
        "key": "ctrl+shift+delete",
        "command": "deleteAllRight",
        "when": "editorTextFocus"
    }
]
```

# Emoji
Inspired by [dannyfritz/commit-message-emoji](https://github.com/dannyfritz/commit-message-emoji)

See also [gitmoji](https://gitmoji.carloscuesta.me/).

|   Commit type              | Emoji                                         |
|:---------------------------|:----------------------------------------------|
| Initial commit             | :tada: `:tada:`                               |
| Version tag                | :bookmark: `:bookmark:`                       |
| New feature                | :sparkles: `:sparkles:`                       |
| Bugfix                     | :bug: `:bug:`                                 |
| Metadata                   | :card_index: `:card_index:`                   |
| Documentation              | :books: `:books:`                             |
| Documenting source code    | :bulb: `:bulb:`                               |
| Performance                | :racehorse: `:racehorse:`                     |
| Cosmetic                   | :lipstick: `:lipstick:`                       |
| Tests                      | :rotating_light: `:rotating_light:`           |
| Adding a test              | :white_check_mark: `:white_check_mark:`       |
| Make a test pass           | :heavy_check_mark: `:heavy_check_mark:`       |
| General update             | :zap: `:zap:`                                 |
| Improve format/structure   | :art: `:art:`                                 |
| Refactor code              | :hammer: `:hammer:`                           |
| Removing code/files        | :fire: `:fire:`                               |
| Continuous Integration     | :green_heart: `:green_heart:`                 |
| Security                   | :lock: `:lock:`                               |
| Upgrading dependencies     | :arrow_up: `:arrow_up:`                       |
| Downgrading dependencies   | :arrow_down: `:arrow_down:`                   |
| Lint                       | :shirt: `:shirt:`                             |
| Translation                | :alien: `:alien:`                             |
| Text                       | :pencil: `:pencil:`                           |
| Critical hotfix            | :ambulance: `:ambulance:`                     |
| Deploying stuff            | :rocket: `:rocket:`                           |
| Fixing on MacOS            | :apple: `:apple:`                             |
| Fixing on Linux            | :penguin: `:penguin:`                         |
| Fixing on Windows          | :checkered_flag: `:checkered_flag:`           |
| Work in progress           | :construction:  `:construction:`              |
| Adding CI build system     | :construction_worker: `:construction_worker:` |
| Analytics or tracking code | :chart_with_upwards_trend: `:chart_with_upwards_trend:` |
| Removing a dependency      | :heavy_minus_sign: `:heavy_minus_sign:`       |
| Adding a dependency        | :heavy_plus_sign: `:heavy_plus_sign:`         |
| Docker                     | :whale: `:whale:`                             |
| Configuration files        | :wrench: `:wrench:`                           |
| Package.json in JS         | :package: `:package:`                         |
| Merging branches           | :twisted_rightwards_arrows: `:twisted_rightwards_arrows:` |
| Bad code / need improv.    | :hankey: `:hankey:`                           |
| Reverting changes          | :rewind: `:rewind:`                           |
| Breaking changes           | :boom: `:boom:`                               |
| Code review changes        | :ok_hand: `:ok_hand:`                         |
| Accessibility              | :wheelchair: `:wheelchair:`                   |
| Move/rename repository     | :truck: `:truck:`                             |
| Other                      | [Be creative](http://www.emoji-cheat-sheet.com/)  |
