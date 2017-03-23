# Enterprise Platforms 
#### `Windows Network Environments`  [![GitHub release](https://img.shields.io/github/release/qubyte/rubidium.svg?style=plastic)](https://github.com/dataweapons/winthirtytwo/tree/v1.1)  [![Website](https://img.shields.io/website-up-down-blue-red/http/shields.io.svg?style=plastic)](http://winthirtytwo.gitlab.dataweapons.org)     [![GitHub license](https://img.shields.io/badge/license-AGPL-blue.svg?style=plastic)](https://raw.githubusercontent.com/dataweapons/winthirtytwo/master/LICENSE) 
 
### Abstract
Core protocols and systems deployed throughout an Enterprise environment implement encryption and other capabilities using [x509] public-key [certificates], [RADIUS], IEEE [8021x], [WPA2-EAP] / [EAP-TLS]

```bash
$ cd dillinger
$ npm install -d
$ node app
```

For production environments...

```bash
$ npm install --production
$ npm run predeploy
$ NODE_ENV=production node app
```

### Plugins

Dillinger is currently extended with the following plugins. Instructions on how to use them in your own application are linked below.

| Component | Repository |
| ------ | ------ |
| PKI | [README.md] [git-pki-repo] |
| PowerShell | [README.md] [git-psh3ll-repo] |
| WIN32 | [README.md] [git-win32-repo] |
| ADCS | [README.md] [git-adcs-repo] |


### Development

First Tab:
```sh
$ node app
```

Second Tab:
```sh
$ gulp watch
```

(optional) Third:
```sh
$ karma test
```
#### Building for source
For production release:
```sh
$ gulp build --prod
```
Generating pre-built zip archives for distribution:
```sh
$ gulp build dist --prod
```

[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)

  
   [dataweapons]: <https://www.dataweapons.org>
   [WIFI]: <https://www.wi-fi.org>
   [x509]: <https://en.wikipedia.org/wiki/X.509>
   [enroll]: <https://enroll.dataweapons.org/certsrv/>
   [Core Infrastructure]: <https://github.com/dataweapons/dillinger>
   [certificates]: <https://en.wikipedia.org/wiki/Public_key_certificate>
   [RADIUS]: <https://en.wikipedia.org/wiki/RADIUS>
   [SMTPS]: <https://en.wikipedia.org/wiki/SMTPS>
   [WPA2-EAP]: <https://en.wikipedia.org/wiki/Extensible_Authentication_Protocol>
   [DNSSEC]: <https://en.wikipedia.org/wiki/DNSSEC>
   [IPSEC]: <https://en.wikipedia.org/wiki/IPSEC>
   [pki]: <http://pki.dataweapons.org/pki>
   [EAP-TLS]: <https://en.wikipedia.org/wiki/Extensible_Authentication_Protocol#EAP-TLS>
   [8021x]: <https://en.wikipedia.org/wiki/IEEE_802.1X>
   [SCEP]: <https://www.ietf.org/id/draft-gutmann-scep-05.txt>
   [NDES]: <http://aka.ms/ndes>
   [CES]:<https://technet.microsoft.com/en-us/library/hh831822(v=ws.11).aspx>
   [CEP]: <https://technet.microsoft.com/en-us/library/hh831625(v=ws.11).aspx>
   [ADCS]: <https://technet.microsoft.com/en-us/library/hh831574(v=ws.11).aspx>
   [git-pki-repo]: <https://github.com/dataweapons/docs/enterprise/pki.git>
   [git-wlan-repo]: <https://github.com/dataweapons/docs/enterprise/wlan.git>
   [git-adcs-repo]: <https://github.com/dataweapons/win32/adcs.git>
   [git-psh3ll-repo]: <http://psh3ll.gitlab.dataweapons.org/>
   [git-win32-repo]: <http://winthirtytwo.gitlab.dataweapons.org/>
   [Environmental Impact Statement]: <https://github.com/dataweapons/pki/eis.aspx>
   [df1]: <http://daringfireball.net/projects/markdown/>
   [markdown-it]: <https://github.com/markdown-it/markdown-it>
   [Ace Editor]: <http://ace.ajax.org>
   [node.js]: <http://nodejs.org>
   [Twitter Bootstrap]: <http://twitter.github.com/bootstrap/>
   [jQuery]: <http://jquery.com>
   [@tjholowaychuk]: <http://twitter.com/tjholowaychuk>
   [express]: <http://expressjs.com>
   [AngularJS]: <http://angularjs.org>
   [Gulp]: <http://gulpjs.com>
   

