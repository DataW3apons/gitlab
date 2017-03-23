# Enterprise Platform Management
### Wireless Local Area Networks (WLANs)

[![Solid](http://www.wi-fi.org/sites/all/themes/wfa/assets/images/WFA_Alliance_Flat_Web_LR.png)](http://www.wi-fi.org/)

### Abstract
Core protocols and systems deployed throughout an Enterprise environment implement encryption and other capabilities using [x509] public-key [certificates].

  - [RADIUS]
  - IEEE [8021x]
  - [WPA2-EAP] / [EAP-TLS]



> The overriding design goal for Markdown's
> formatting syntax is to make it as readable
> as possible. The idea is that a
> Markdown-formatted document should be
> publishable as-is, as plain text, without
> looking like it's been marked up with tags
> or formatting instructions.

```sh
$ cd dillinger
$ npm install -d
$ node app
```

For production environments...

```sh
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
### Docker

```sh
cd dillinger
docker build -t dataweapons/dillinger:${package.json.version}
```
This will create the dillinger image and pull in the necessary dependencies. Be sure to swap out `${package.json.version}` with the actual version of Dillinger.

Once done, run the Docker image and map the port to whatever you wish on your host. In this example, we simply map port 8000 of the host to port 80 of the Docker (or whatever port was exposed in the Dockerfile):

```sh
docker run -d -p 8000:8080 --restart="always" <youruser>/dillinger:${package.json.version}
```

Verify the deployment by navigating to your server address in your preferred browser.

```sh
127.0.0.1:8000
```


[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)

  
   [dataweapons]: <https://www.dataweapons.org>
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
   
