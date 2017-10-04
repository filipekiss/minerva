# Emoji Guide

This project uses emoji to help, at a glance, quickly understand what changes a single commit is
making.

## Adding emojis to your commits

Avoid adding the unicode character to the commit message. This is to prevent problems when rendering
the commit message in systems that may not yet support emoji. This also allows for easier filtering
the commits on the command line, since you can `grep` for the emoji name instead of the unicode
character.

## How many emoji are too many?

Try to keep at only two emojis per commit title. If you wish, you may add emojis to the description,
but it's not required. If you think no emoji applies to your commit, you're free to leave it out
(and maybe suggest a new emoji).

## What does it mean?

Here's the list of all emojis you may encounter in our commits. They're listed alphabetically by
their description and their code is right next to them.


Description | Emoji | Emoji Code
--- | :---: | ---
Adding CI build system. | :construction_worker: | `:construction_worker:`
Adding Logging | :speaker: | `:speaker:`
Adding a dependency. | :heavy_plus_sign: | `:heavy_plus_sign:`
Adding analytics or tracking code. | :chart_with_upwards_trend: | `:chart_with_upwards_trend:`
Adding or updating assets. | :bento: | `:bento:`
Adding or updating license. | :page_facing_up: | `:page_facing_up:`
Adding tests | :umbrella: | `:umbrella:`
Anything related to Deployments/DevOps | :rocket: | `:rocket:`
Change file structure | :tractor: | `:tractor:`
Changing configuration files. | :wrench: | `:wrench:`
Customer requested application Customization, with @HACK Comment Tag | :ribbon: | `:ribbon:`
Downgrading dependencies. | :arrow_down: | `:arrow_down:`
Fixing CI Build. | :green_heart: | `:green_heart:`
Fixing a bug. | :bug: | `:bug:`
Fixing security issues. | :lock: | `:lock:`
Fixing something on Android. | :robot: | `:robot:`
Fixing something on Linux. | :penguin: | `:penguin:`
Fixing something on Windows. | :checkered_flag: | `:checkered_flag:`
Fixing something on iOS. | :green_apple: | `:green_apple:`
Fixing something on macOS. | :apple: | `:apple:`
Fixing typos. | :pencil2: | `:pencil2:`
Forward-porting features from an older version/branch | :fast_forward: | `:fast_forward:`
Generic Database specific (Migrations, Scripts, Extensions, ...) | :bank: | `:bank:`
Hotfix. | :ambulance: | `:ambulance:`
Improving accessibility. | :wheelchair: | `:wheelchair:`
Improving performance. | :zap: | `:zap:`
Improving the format/structure of the code | :art: | `:art:`
Initial commit. | :tada: | `:tada:`
Internationalization and localization. | :globe_with_meridians: | `:globe_with_meridians:`
Introducing breaking changes. | :boom: | `:boom:`
Introducing new features. | :sparkles: | `:sparkles:`
Merge files | :handshake: | `:handshake:`
Merging branches. | :twisted_rightwards_arrows: | `:twisted_rightwards_arrows:`
MongoDB Database specific (Migrations, Scripts, Extensions, ...) | :leaves: | `:leaves:`
Moving or renaming files. | :truck: | `:truck:`
MySQL Database specific (Migrations, Scripts, Extensions, ...) | :dolphin: | `:dolphin:`
New Idea, with @IDEA Comment Tag | :bulb: | `:bulb:`
Performing database related changes. | :card_file_box: | `:card_file_box:`
Performing minor changes/fixing the code or language | :pencil: | `:pencil:`
PostgreSQL Database specific (Migrations, Scripts, Extensions, ...) | :elephant: | `:elephant:`
Refactoring code. | :hammer: | `:hammer:`
Releasing / Version tags. | :bookmark: | `:bookmark:`
Removing a dependency. | :heavy_minus_sign: | `:heavy_minus_sign:`
Removing code or files. | :fire: | `:fire:`
Removing linter warnings. | :rotating_light: | `:rotating_light:`
Reverting changes. | :rewind: | `:rewind:`
Updating code due to code review changes. | :ok_hand: | `:ok_hand:`
Updating code due to external API changes. | :alien: | `:alien:`
Updating compiled files or packages. | :package: | `:package:`
Updating text and literals. | :speech_balloon: | `:speech_balloon:`
Updating the UI and style files. | :lipstick: | `:lipstick:`
Upgrading dependencies. | :arrow_up: | `:arrow_up:`
W.I.P - Work in progress. | :construction: | `:construction:`
Work about Docker. | :whale: | `:whale:`
Writing bad code that needs to be improved. | :hankey: | `:hankey:`
Writing docs | :books: | `:books:`
