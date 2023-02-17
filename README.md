
### Installation by composer
###
```
{
    "require": {
      "lucasaguiar86/yii2-sftp-phpseclib": "dev-main"
   }
}
```
 ### or
 ###

>$ composer require lucasaguiar86/yii2-sftp-phpseclib

### USAGE
###
```
'components' => [
      ...
      'sftp' => [
          "class" => 'Datassential\sftp\SFtpManager',
          "settings"=>[
              'port'=>22,
              'timeout'=>10
            ]
       ],
 ],
 
$sftp = Yii::$app->sftp
$sftp->connect("host","user","pass");
echo $sftp->isConnected();
```

## Documentation

* [Documentation / Manual](http://phpseclib.sourceforge.net/)
* [API Documentation](https://api.phpseclib.org/master/)



License
----

MIT
#
