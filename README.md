# CODIFICATION
To obfuscate your plugin by just follow the steps on this site: https://www.php-obfuscator.com/?demo, now to put a system to verify by IP follow the steps below.

## AntiLeak
In ```onEnable()``` you must define the code:
```php
PluginEncriptEnable::generateToken($this, "BuyerServerIp:BuyerServerPort");
PluginEncriptEnable::checkPlugin($this);
```

## Extra Functions
```php
PluginEncriptEnable::getToken((Plugin) $this); //Get token from a plugin
PluginEncriptEnable::isValidToken((Plugin) $this); //Check if the token is valid, return Bool.
```

## Import
To do all this it is necessary to import the use:
```php
use LadinoXx\LoaderCloudKodePlugin\PluginEncriptEnable;
```
