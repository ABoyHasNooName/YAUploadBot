# Yet Another UploadBot

Telegram bot able to upload large file.

## Installation

YAUploadBot requires [PHP](http://php.net/downloads.php) >= 5.6.0 and [Composer](https://getcomposer.org/) to run.

### Dependencies installation

To be able to run tele_uploader, you **must** install all the dependencies listed in [composer.json](/composer.json); to do that, type:

```sh
$ composer install
```

This process can take a while...

## Configuration

After all dependencies are satisfied, you can start to configure the environment variables.

For convenience, I've listed them inside the [config.php](/config.php) file so that the only thing you have to do is open it and fill with your keys.

### Keys meaning

We have just five keys:

- BOT_TOKEN     : the unique token generated by [@BotFather](https://t.me/BotFather)
- APP_ID        : Get your own token from my.telegram.org 
- API_HASH      : Get your own token from my.telegram.org
- BOT_SESSION   : Most probably, you won't need to change this. This location is where your login session is stored
- TMP_DOWNLOADS : The directory where the downloaded files should be stored

## Run!

Now we're ready to execute the bot!

Let's import the environment variable, with:

```sh
$ cp config.sample.php config.php
```

and then...run!

```sh
$ php bot.php
```

## Credits

A special thanks to [Daniil Gentili](https://daniil.it/) aka [danog](https://github.com/danog) that created [MadelineProto](https://github.com/danog/MadelineProto).
