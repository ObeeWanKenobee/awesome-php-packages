# Awesome-PHP-Packages
Awesome Collective: Useful composer packages

### *Ahem.. out check. 0.. 1.. 2.. 3..
This project started because I'm tired browsing around packagist looking for useful packages.

PRs are welcome as long as the changes are of course useful.

This project also contains tips and tricks about composer.

That's all.

#### Special thanks to -> Composer (of course), Drupal's composer.json, Laravel's composer.json, and so on. // Just add some copyrights in here so I wont get into trouble someday

```json
{
	"name": "Awesome PHP Packages",
	"homepage": "https://packagist.org/",
	"keywords": ["Awesome list", "Curated list", "php"],
	"description": "OpenSource Collective: Useful composer packages",
	"version": "1.0.1",
	"type": "project",
	"license": "The Unlicensed",
	"authors": [
		{
			"name": "Emmanuel Lanuzo",
			"homepage": "https://emmanuellanuzo.com",
			"role": "Founder"
		},
		{
			"name": "just add yo name here",
			"homepage": "websiteofcourse.com",
			"role": "Contributor",
		}
	],
	"config": {
		"github-oauth": {
			"github.com": "abcdefghijklmnopqrstuvwxyz012345678910"
		},
		"gitlab-oauth": {
			"gitlab.com": "abcdefghijklmnopqrstuvwxyz012345678910"
		},
		"gitlab-token": {
			"github.com": "abcdefghijklmnopqrstuvwxyz012345678910"
		},
		"github.com": {
			"username": "kenobee",
			"password": "hellothere"
		},
		"gitlab.com": {
			"username": "kenobee",
			"password": "hellothere"
		},
		{
		"bitbucket.org": {
				"consumer-key": "myKey",
				"consumer-secret": "mySecret"
			}
		},
		"abandoned": true,
		"apcu-autoloader": true,
		"archive-format": tar,
		"autoloader-suffix": "nani",
		"bin-compat": "full",
		"bin-dir": "anywhere",
		"cache-dir": "caches",
		"cache-files-dir": "files",
		"cache-repo-dir": "repos",
		"cache-vcs-dir": "vcs",
		"cache-files-ttl": 86400,
		"cache-files-maxsize": 300MiB,
		"cafile": "lo/ca/ti/on/he/he/cafile.ca",
		"capath": "lo/ca/ti/on/he/he/cafile.ca",
		"classmap-authoritative": true,
		"data-dir": "somewhere/deep",
		"disable-tls": false,
		"discard-changes": true,
		"github-expose-hostname": true,
		"github-protocols": ["https", "ssh", "git"],
		"htaccess-protect": true,
		"http-basic": {"example.org": {
				"username": "oneesan",
				"password": "labsoniichan"
			}
		},
		"notify-on-install": true,
		"optimize-autoloader": true,
		"prepend-autoloader": true,
		"process-timeout": 0,
		"secure-http": true,
		"sort-packages": true,
		"store-auths": true,
		"use-include-path": true,
		"vendor-dir": "everywhere",
		"platform": {
			"php": "7.2.6",
			"ext-amqp": "7.2.6",
			"ext-apc": "7.2.6",
			"ext-apcu": "7.2.6",
			"ext-dba": "7.2.6",
			"ext-ds": "7.2.6",
			"ext-event": "7.2.6",
			"ext-gd2": "7.2.6",
			"ext-gmagick": "7.2.6",
			"ext-gmp": "7.2.6",
			"ext-imagick": "7.2.6",
			"ext-intl": "7.2.6",
			"ext-libsodium": "7.2.6",
			"ext-maxminddb": "7.2.6",
			"ext-mcrypt": "7.2.6",
			"ext-memcache": "7.2.6",
			"ext-memcached": "7.2.6",
			"ext-mongo": "7.2.6",
			"ext-mongodb": "7.2.6",
			"ext-pcntl": "7.2.6",
			"ext-phpiredis": "7.2.6",
			"ext-posix": "7.2.6",
			"ext-redis": "7.2.6",
			"ext-soap": "7.2.6",
			"ext-sodium": "7.2.6",
			"ext-uopz": "7.2.6",
			"ext-uuid": "7.2.6",
			"ext-wincache": "7.2.6",
			"ext-xcache": "7.2.6",
			"ext-xdebug": "7.2.6",
			"ext-xsl": "7.2.6"
		},
		"preferred-install": {
			"*": "dist"
		}
		"fxp-asset": {
			"enabled": false,
			"installer-paths": {
				"npm-asset-library": "omaewa",
				"bower-asset-library": "shindeiru"
			}
		}
	},
	"repositories": [
		{
			"type": "composer",
			"url": "https://asset-packagist.org"
		},
		{
			"type": "vcs",
			"url": "https://github.com"
		},
		{
			"type": "vcs",
			"url": "https://gitlab.com"
		},
		{
			"type": "vcs",
			"url": "https://bitbucket.org"
		}
	],
	"extra": {
		"_readme": [
			"readme niichan"
		],
		"merge-plugin": {
			"include": [
				"another/one.json",
				"composer2.json"
			],
			"recurse": true,
			"replace": false,
			"merge-extra": false
		},
		"installer-paths": {
			"core": ["type:drupal-core"],
				"modules/contrib/{$name}": ["type:drupal-module"]
			}
		},
		"autoload": {
			"psr-4": {
				"Name\\space\\Class\\": "lo/ca/ti/on"
			},
			"classmap": [
				"phps/php.php"
			]
		},
		"scripts": {
			"pre-autoload-dump": "Name\\space\\Class\\Composer::preAutoloadDump",
			"post-autoload-dump": "Name\\space\\Class\\Composer::ensureHtaccess",
			"post-package-install": "Name\\space\\Class\\Composer::vendorTestCodeCleanup",
			"phpcs": "phpcs --standard=core/phpcs.xml.dist --runtime-set installed_paths $($COMPOSER_BINARY config vendor-dir)/coder/coder_sniffer --",
			"phpcbf": "phpcbf --standard=core/phpcs.xml.dist --runtime-set installed_paths $($COMPOSER_BINARY config vendor-dir)/coder/coder_sniffer --"
		}
	}
	"minimum-stability": "dev",
	"prefer-stable": true,
	"require": {
		"adaptive/php-text-difference": ">=1.0.3",
		"adbario/php-dot-notation": ">=2",
		"adbario/php-encrypter": ">=1",
		"albaraam/php-gcm-apns": ">=1",
		"ambroisemaupate/date-to-sentence": ">=1.2",
		"appstract/lush-http": ">=0.5.4",
		"arthurkushman/coossions": ">=1.1.1",
		"atrapalo/urlcrypt": ">=1.0.1",
		"azuyalabs/yasumi": ">=1.8",
		"barracudanetworks/archivestream-php": ">=1.0.5",
		"basekit/colorworks": ">=1",
		"blobfolio/blob-common": ">=8",
		"botman/botman": ">=2.3.3",
		"cartalyst/converter": ">=3.0.1",
		"cidram/cidram": ">=1.6",
		"coduo/php-humanizer": ">=2",
		"coduo/php-matcher": ">=3.1",
		"cogpowered/finediff": ">=0.3.1",
		"composer/ca-bundle": ">=1.1.1",
		"danielstjules/php-pretty-datetime": "dev-master",
		"danielstjules/stringy": ">=3.1",
		"dater/dater": ">=2.0.3",
		"dawood/phpchromepdf": ">=1.3",
		"dawood/phpscreenrecorder": ">=1.4",
		"dawood/wmb-scrapper": ">=1.1",
		"defuse/php-encryption": ">=2.2",
		"demi/safe-text": ">=1.0.2",
		"diversen/http-send-file": ">=2.0.3",
		"doctrine/dbal": ">=2.7",
		"dragonmantank/cron-expression": ">=2.1",
		"egulias/email-validator": ">=2.1.4",
		"embed/embed": ">=3.3.3",
		"endroid/qr-code": ">=3.2.12",
		"evozon-php/tissue": "dev-master",
		"fabpot/goutte": ">=3.2.2",
		"facile-it/doctrine-mysql-come-back": ">=1.6.5",
		"fightbulc/moment": ">=1.26.10",
		"filp/whoops": ">=2.1.14",
		"fzaninotto/faker": ">=1.7.1",
		"genkgo/mail": ">=2.5.1",
		"genkgo/push": ">=1",
		"geoip2/geoip2": ">=2.9",
		"giggsey/libphonenumber-for-php": ">=8.9.7",
		"gladcodes/keygen": ">=1.1.1",
		"gregwar/image": ">=2.0.22",
		"guzzlehttp/guzzle": ">=6.3.3",
		"guzzlehttp/promises": ">=1.3.1",
		"guzzlehttp/psr7": ">=1.4.2",
		"hashids/hashids": ">=3",
		"hassankhan/config": ">=1.0.1",
		"ilya/belt": ">=2.1.1",
		"ilya/collection": ">=1",
		"imagine/imagine": ">=0.7.1",
		"imanee/imanee": ">=1.2.2",
		"intervention/image": ">=2.4.2",
		"intervention/imagecache": ">=2.3.3",
		"ircmaxell/random-lib": ">=1.2",
		"james-heinrich/getid3": "1.9.x-dev",
		"jaybizzle/crawler-detect": ">=1.2.63",
		"jbroadway/urlify": "1.1.0-stable",
		"jenssegers/date": ">=3.4",
		"jeroendesloovere/geolocation-php-api": ">=2.1",
		"jeroendesloovere/vcard": ">=1.6",
		"jkuchar/bigfiletools": ">=2",
		"jkuchar/filedownloader": ">=2",
		"josantonius/cookie": ">=1.1.6",
		"josantonius/errorhandler": ">=1.1.8",
		"josantonius/file": ">=1.1.7",
		"josantonius/httpstatuscode": ">=1.1.6",
		"josantonius/ip": ">=1.1.7",
		"josantonius/mimetype": ">=1.1.7",
		"josantonius/request": ">=1.1.7",
		"josantonius/url": ">=1.2.1",
		"jproof/jybrid": ">=0.7.7",
		"jstewmc/detect-environment": ">=2",
		"jstewmc/encode-file": ">=0.2",
		"jstewmc/expand-abbreviations": ">=1",
		"jstewmc/get-ip": ">=0.1.0",
		"jstewmc/php-helpers": ">=0.1.1",
		"jstewmc/validate-file-size": ">=0.1",
		"kasp3r/link-preview": ">=2",
		"katzien/php-mime-type": ">=2.1",
		"khr/php-mcurl-client": ">=3.1",
		"knplabs/knp-snappy": ">=1.0.4",
		"lambdish/phunctional": ">=1.0.4",
		"laravolt/avatar": ">=2.0.4",
		"lasserafn/php-hexer": ">=1.05",
		"lasserafn/php-initial-avatar-generator": ">=2.3",
		"lasserafn/php-initials": ">=2.20",
		"lasserafn/php-string-script-language": ">=0.1",
		"league/flysystem": ">=1.0.45",
		"league/flysystem-memory": ">=1",
		"league/flysystem-sftp": ">=1.0.15",
		"lightster/assetrinc": ">=0.4.1",
		"lightster/named-sprintf": ">=0.1.2",
		"limonte/google-safebrowsing": ">=0.1",
		"limonte/spam-link-analyser": ">=0.1.1",
		"maennchen/zipstream-php": ">=0.5.2",
		"malios/php-to-ascii-table": ">=1.0.1",
		"marc1706/fast-image-size": ">=1.1.4",
		"marcelklehr/link-preview": ">=1.2.11",
		"marcoazn89/http-wrapper": ">=2.1.1",
		"markrogoyski/ipv4-subnet-calculator": ">=2.1",
		"markrogoyski/math-php": ">=0.43",
		"martijnc/php-csp": ">=1.0.2",
		"matthiasmullie/minify": ">=1.3.60",
		"mdf/php-url-resolver": "dev-master",
		"merlinthemagic/mts": ">=1.1.1",
		"microweber/screen": ">=1.0.6",
		"misd/linkify": ">=1.1.2",
		"mjaschen/phpgeo": ">=2.0.2",
		"mobiledetect/mobiledetectlib": ">=2.8.32",
		"monolog/monolog": ">=1.23",
		"moontoast/math": ">=1.1.2",
		"mormat/php-formula-interpreter": ">=1",
		"mossadal/math-parser": ">=1.3.13",
		"mostka/defer": "dev-master",
		"mostka/hgtreader": "dev-master",
		"mpdf/mpdf": ">=7.1",
		"mpratt/relativetime": ">=1.5.4",
		"mso/idna-convert": ">=1.1",
		"nelexa/zip": ">=3.1.5",
		"nesbot/carbon": ">=1.29.2",
		"nette/http": ">=2.4.9",
		"nette/mail": ">=2.4.5",
		"nette/robot-loader": ">=3.0.x-dev",
		"nette/utils": ">=2.5.2",
		"nikic/fast-route": ">=1.3",
		"nikic/phlexy": ">=0.1",
		"noprotocol/php-mysql-aes-crypt": ">=2.0.1",
		"ollyxar/websockets": ">=2.1.1",
		"opis/data-store": ">=1.0.1",
		"opis/pattern": ">=1",
		"paragonie/certainty": ">=2.1",
		"paragonie/constant_time_encoding": ">=2.2.2",
		"paragonie/cookie": ">=3.2",
		"paragonie/halite": ">=4.4.2",
		"paragonie/ionizer": ">=0.3",
		"paragonie/password_lock": ">=3.0.1",
		"paragonie/random_compat": ">=2.0.15",
		"paragonie/sodium_compat": ">=1.6.3",
		"paragonie/stern": "dev-master",
		"pavelsterba/http-exceptions": ">=1.1",
		"peppeocchi/php-cron-scheduler": ">=2.3.2",
		"php-curl-class/php-curl-class": ">=8.1",
		"php-di/php-di": ">=5.4.6",
		"phpcollection/phpcollection": ">=0.5",
		"phpfanatic/clarifai": ">=2.0.1",
		"phpmailer/phpmailer": ">=6.0.5",
		"phpoffice/phppresentation": ">=0.9",
		"phpoffice/phpspreadsheet": ">=1.3.1",
		"phpoffice/phpword": ">=0.14",
		"phpwhois/phpwhois": ">=4.2.5",
		"piwik/device-detector": ">=3.10.2",
		"pragmarx/countries": ">=0.5.8",
		"ps/image-optimizer": ">=1.2",
		"ptcong/easyrequest": ">=1.0.6",
		"punic/punic": ">=3.1",
		"ramsey/uuid": ">=3.7.3",
		"regex-guard/regex-guard": ">=1.1",
		"respect/validation": ">=1.1.16",
		"rhubarbphp/module-csrfprotection": ">=1.0.5",
		"rinvex/country": ">=3.1",
		"rinvex/language": ">=2",
		"rinvex/university": ">=1.1.1",
		"roave/security-advisories": "dev-master",
		"savvot/random": ">=0.3",
		"sdboyer/frozone": ">=1.0.2",
		"sdboyer/gliph": ">=0.7",
		"sebastian/comparator": ">=3.0.1",
		"sebastian/diff": ">=3.0.1",
		"selvinortiz/flux": ">=0.5.3",
		"selvinortiz/gossip": ">=1",
		"sinergi/browser-detector": ">=6.1.2",
		"sinergi/token": ">=0.1",
		"smalot/pdfparser": ">=0.12",
		"smsapi/php-client": ">=1.8.7",
		"solaris/php-moon-phase": ">=1.1.1",
		"spatie/browsershot": ">=3.22.1",
		"spatie/email-concealer": ">=1.0.1",
		"spatie/emoji": ">=1.0.6",
		"spatie/geocoder": ">=3.3.1",
		"spatie/image-optimizer": ">=1.0.14",
		"spatie/opening-hours": ">=1.6",
		"spatie/pdf-to-image": ">=1.8",
		"spatie/pdf-to-text": ">=1.1",
		"spatie/regex": ">=1.3",
		"spatie/schema-org": ">=1.6",
		"spatie/ssl-certificate": ">=1.12.7",
		"spatie/url": ">=1.3",
		"spatie/url-signer": ">=1.0.2",
		"spomky-labs/base64url": ">=1.0.2",
		"stefangabos/zebra_curl": ">=1.3.5",
		"stefangabos/zebra_session": ">=2.1.8",
		"stil/gif-endec": ">=0.2",
		"sun/country": ">=1.3",
		"sun/filesystem": ">=1.3",
		"swiftmailer/swiftmailer": ">=6.0.2",
		"symfony/polyfill-util": ">=1.8",
		"tburry/pquery": ">=1.1.1",
		"theiconic/name-parser": ">=1.2",
		"theiconic/php-ga-measurement-protocol": ">=2.7.1",
		"tracy/tracy": ">=2.5",
		"ua-parser/uap-php": ">=3.5",
		"validator/livr": "dev-master",
		"vanilla/htmlawed": ">=2.2.4.1",
		"victorybiz/geoip-location": ">=1.0.2",
		"vlucas/valitron": ">=1.4.3",
		"voku/anti-xss": ">=4.1.1",
		"voku/email-check": ">=3",
		"voku/html-min": ">=3.0.3",
		"voku/portable-utf8": ">=5.0.6",
		"warriorxk/phpwebsockets": ">=2.0.1",
		"webmozart/assert": ">=1.3",
		"webmozart/path-util": ">=2.3",
		"whichbrowser/parser": ">=2.0.32",
		"yetiforce/csrf-magic": ">=1.0.8",
		"yzalis/identicon": ">=1.2",
		"zendframework/zendframework": ">=3",
		"zendframework/zendservice-recaptcha": ">=3.1",
		"zhenhao/smaz": ">=1.1.1"
	},
	"require-dev": {
		"phpunit": ">=7"
	},
	"replace": {
		"laravel/laravel": ">=5.7"
	}
}
```
