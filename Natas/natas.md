# Over The Wire - Natas

## Level 0

* View Source
* gtVrDuiDfck831PqWsLEZy5gyDz1clto

## Level 1

* Mac: Command + Option + U
* ZluruAthQk7Q2MqmDeTiUij2ZvWy2mBi

## Level 2

* View Source
* Notice img src
* Go to http://natas2.natas.labs.overthewire.org/files/users.txt
* sJIJNW6ucpu6HPZ1ZAchaDtwd7oGrD14

## Level 3

* View Source
* Notice Google Hint
  * File that makes search engines not look at certain pages?
* http://natas3.natas.labs.overthewire.org/robots.txt
* http://natas3.natas.labs.overthewire.org/s3cr3t/
* http://natas3.natas.labs.overthewire.org/s3cr3t/users.txt
* Z9tkRkWmpt9Qr7XrR5jWRkgOU901swEZ

## Level 4

* Burp Suit
* Proxy to 127.0.0.1:8080
* Intercept on
* Refresh Natas page
* Update referer to 'http://natas5.natas.labs.overthewire.org/'
* iX6IOfmpN7AYOQGPwtn3fXpbaJVJcHfq 

## Level 5

* Burp Suit
* Intercept on
* Refresh page
* Set "loggedin=" to 1
* aGoY4q2Dc6MgDq4oL4YtoKtyAg9PeHa1

## Level 6

* View Source
* Notice "include..."
* Go to "http://natas6.natas.labs.overthewire.org/includes/secret.inc"
* View page source
* $secret = "FOEIUWGHFEEUHOFUOIU";
* Submit secret
* 7z3hEENjQtflzgnT29q7wAvMNfZdh0i9

## Level 7

* View Source
* http://natas7.natas.labs.overthewire.org/index.php?page=/etc/natas_webpass/natas8
* DBfUBfqQG69KvJvJ1iAbMoIpwSNQ9bWe

## Level 8

* View sourcecode
* Notice PHP script
* bin2hex(strrev(base64_encode($secret)));
* Reverse it to: base64_decode(strrev(hex2bin("3d3d516343746d4d6d6c315669563362")));
* Run in PHP sandbox
* Input secret: oubWYf2kBq
* W0mMhUcRRnG8dcghE4qvk3JA9lGt8nDl

## Level 9

*
