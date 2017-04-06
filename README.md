# api documentation for  [express-useragent (v1.0.7)](https://github.com/biggora/express-useragent/)  [![npm package](https://img.shields.io/npm/v/npmdoc-express-useragent.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-express-useragent) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-express-useragent.svg)](https://travis-ci.org/npmdoc/node-npmdoc-express-useragent)
#### ExpressJS/Connect/TrinteJS user-agent middleware exposing

[![NPM](https://nodei.co/npm/express-useragent.png?downloads=true)](https://www.npmjs.com/package/express-useragent)

[![apidoc](https://npmdoc.github.io/node-npmdoc-express-useragent/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-express-useragent_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-express-useragent/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-express-useragent/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-express-useragent/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Alexey Gordeyev",
        "email": "aleksej@gordejev.lv",
        "url": "https://github.com/biggora"
    },
    "bugs": {
        "url": "https://github.com/biggora/express-useragent/issues"
    },
    "contributors": [
        {
            "name": "Kacper Glowacki",
            "url": "https://github.com/kacperus"
        },
        {
            "name": "elisee",
            "url": "https://github.com/elisee"
        },
        {
            "name": "Bitdeli Chef",
            "url": "https://github.com/bitdeli-chef"
        },
        {
            "name": "Nicolas Tobo",
            "url": "https://github.com/nicolastobo"
        },
        {
            "name": "Samy Pess�",
            "url": "https://github.com/SamyPesse"
        },
        {
            "name": "Artem Nezvigin",
            "url": "https://github.com/artnez"
        },
        {
            "name": "Josh Dickson",
            "url": "https://github.com/joshdickson40"
        }
    ],
    "dependencies": {},
    "description": "ExpressJS/Connect/TrinteJS user-agent middleware exposing",
    "devDependencies": {
        "bower": "*",
        "express": ">= 3.0.0",
        "grunt": "*",
        "grunt-contrib-clean": "*",
        "grunt-contrib-uglify": "*",
        "jshint": "*",
        "load-grunt-tasks": "^3.2.0",
        "nodeunit": "*"
    },
    "directories": {
        "lib": "lib",
        "test": "test"
    },
    "dist": {
        "shasum": "153de647e5a5d05c4ec1b4172794a46bc0d07991",
        "tarball": "https://registry.npmjs.org/express-useragent/-/express-useragent-1.0.7.tgz"
    },
    "engines": {
        "node": ">=0.8"
    },
    "gitHead": "c25499f977266ebaeb6738cf76280077dc672e9a",
    "homepage": "https://github.com/biggora/express-useragent/",
    "keywords": [
        "useragent",
        "connect",
        "express",
        "trinte",
        "browser",
        "compound",
        "middleware"
    ],
    "license": "MIT",
    "main": "./index.js",
    "maintainers": [
        {
            "name": "biggora",
            "email": "aleksej@gordejev.lv"
        }
    ],
    "name": "express-useragent",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/biggora/express-useragent.git"
    },
    "scripts": {
        "build": "grunt build",
        "express": "node test/express.js",
        "http": "node test/http.js",
        "lint": "make lint",
        "test": "nodeunit test/browsers.js test/bots_test.js"
    },
    "version": "1.0.7"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module express-useragent](#apidoc.module.express-useragent)
1.  [function <span class="apidocSignatureSpan">express-useragent.</span>UserAgent ()](#apidoc.element.express-useragent.UserAgent)
1.  [function <span class="apidocSignatureSpan">express-useragent.</span>express ()](#apidoc.element.express-useragent.express)
1.  [function <span class="apidocSignatureSpan">express-useragent.</span>getBrowser (string)](#apidoc.element.express-useragent.getBrowser)
1.  [function <span class="apidocSignatureSpan">express-useragent.</span>getBrowserVersion (string)](#apidoc.element.express-useragent.getBrowserVersion)
1.  [function <span class="apidocSignatureSpan">express-useragent.</span>getOS (string)](#apidoc.element.express-useragent.getOS)
1.  [function <span class="apidocSignatureSpan">express-useragent.</span>getPlatform (string)](#apidoc.element.express-useragent.getPlatform)
1.  [function <span class="apidocSignatureSpan">express-useragent.</span>parse (source)](#apidoc.element.express-useragent.parse)
1.  [function <span class="apidocSignatureSpan">express-useragent.</span>reset ()](#apidoc.element.express-useragent.reset)
1.  [function <span class="apidocSignatureSpan">express-useragent.</span>testAndroidTablet ()](#apidoc.element.express-useragent.testAndroidTablet)
1.  [function <span class="apidocSignatureSpan">express-useragent.</span>testBot ()](#apidoc.element.express-useragent.testBot)
1.  [function <span class="apidocSignatureSpan">express-useragent.</span>testCaptiveNetwork ()](#apidoc.element.express-useragent.testCaptiveNetwork)
1.  [function <span class="apidocSignatureSpan">express-useragent.</span>testCompatibilityMode ()](#apidoc.element.express-useragent.testCompatibilityMode)
1.  [function <span class="apidocSignatureSpan">express-useragent.</span>testKindleFire ()](#apidoc.element.express-useragent.testKindleFire)
1.  [function <span class="apidocSignatureSpan">express-useragent.</span>testMobile ()](#apidoc.element.express-useragent.testMobile)
1.  [function <span class="apidocSignatureSpan">express-useragent.</span>testNginxGeoIP (headers)](#apidoc.element.express-useragent.testNginxGeoIP)
1.  [function <span class="apidocSignatureSpan">express-useragent.</span>testSilk ()](#apidoc.element.express-useragent.testSilk)
1.  [function <span class="apidocSignatureSpan">express-useragent.</span>testSmartTV ()](#apidoc.element.express-useragent.testSmartTV)
1.  [function <span class="apidocSignatureSpan">express-useragent.</span>testTablet ()](#apidoc.element.express-useragent.testTablet)
1.  object <span class="apidocSignatureSpan">express-useragent.</span>Agent
1.  object <span class="apidocSignatureSpan">express-useragent.</span>DefaultAgent
1.  object <span class="apidocSignatureSpan">express-useragent.</span>_Browsers
1.  object <span class="apidocSignatureSpan">express-useragent.</span>_OS
1.  object <span class="apidocSignatureSpan">express-useragent.</span>_Platform
1.  object <span class="apidocSignatureSpan">express-useragent.</span>_Versions
1.  object <span class="apidocSignatureSpan">express-useragent.</span>express_useragent
1.  string <span class="apidocSignatureSpan">express-useragent.</span>version

#### [module express-useragent.express_useragent](#apidoc.module.express-useragent.express_useragent)
1.  [function <span class="apidocSignatureSpan">express-useragent.express_useragent.</span>UserAgent ()](#apidoc.element.express-useragent.express_useragent.UserAgent)



# <a name="apidoc.module.express-useragent"></a>[module express-useragent](#apidoc.module.express-useragent)

#### <a name="apidoc.element.express-useragent.UserAgent"></a>[function <span class="apidocSignatureSpan">express-useragent.</span>UserAgent ()](#apidoc.element.express-useragent.UserAgent)
- description and source-code
```javascript
UserAgent = function () {
    this.version = '1.0.4';
    this._Versions = {
        Edge: /Edge\/([\d\w\.\-]+)/i,
        Firefox: /firefox\/([\d\w\.\-]+)/i,
        IE: /msie\s([\d\.]+[\d])|trident\/\d+\.\d+;.*[rv:]+(\d+\.\d)/i,
        Chrome: /chrome\/([\d\w\.\-]+)/i,
        Chromium: /(?:chromium|crios)\/([\d\w\.\-]+)/i,
        Safari: /version\/([\d\w\.\-]+)/i,
        Opera: /version\/([\d\w\.\-]+)|OPR\/([\d\w\.\-]+)/i,
        Ps3: /([\d\w\.\-]+)\)\s*$/i,
        Psp: /([\d\w\.\-]+)\)?\s*$/i,
        Amaya: /amaya\/([\d\w\.\-]+)/i,
        SeaMonkey: /seamonkey\/([\d\w\.\-]+)/i,
        OmniWeb: /omniweb\/v([\d\w\.\-]+)/i,
        Flock: /flock\/([\d\w\.\-]+)/i,
        Epiphany: /epiphany\/([\d\w\.\-]+)/i,
        WinJs: /msapphost\/([\d\w\.\-]+)/i,
        PhantomJS: /phantomjs\/([\d\w\.\-]+)/i,
        UC: /UCBrowser\/([\d\w\.]+)/i
    };
    this._Browsers = {
        Edge: /edge/i,
        Amaya: /amaya/i,
        Konqueror: /konqueror/i,
        Epiphany: /epiphany/i,
        SeaMonkey: /seamonkey/i,
        Flock: /flock/i,
        OmniWeb: /omniweb/i,
        Chromium: /chromium|crios/i,
        Chrome: /chrome/i,
        Safari: /safari/i,
        IE: /msie|trident/i,
        Opera: /opera|OPR/i,
        PS3: /playstation 3/i,
        PSP: /playstation portable/i,
        Firefox: /firefox/i,
        WinJs: /msapphost/i,
        PhantomJS: /phantomjs/i,
        UC: /UCBrowser/i
    };
    this._OS = {
        Windows10: /windows nt 10\.0/i,
        Windows81: /windows nt 6\.3/i,
        Windows8: /windows nt 6\.2/i,
        Windows7: /windows nt 6\.1/i,
        UnknownWindows: /windows nt 6\.\d+/i,
        WindowsVista: /windows nt 6\.0/i,
        Windows2003: /windows nt 5\.2/i,
        WindowsXP: /windows nt 5\.1/i,
        Windows2000: /windows nt 5\.0/i,
        WindowsPhone81: /windows phone 8\.1/i,
        WindowsPhone80: /windows phone 8\.0/i,
        OSXCheetah: /os x 10[._]0/i,
        OSXPuma: /os x 10[._]1(\D|$)/i,
        OSXJaguar: /os x 10[._]2/i,
        OSXPanther: /os x 10[._]3/i,
        OSXTiger: /os x 10[._]4/i,
        OSXLeopard: /os x 10[._]5/i,
        OSXSnowLeopard: /os x 10[._]6/i,
        OSXLion: /os x 10[._]7/i,
        OSXMountainLion: /os x 10[._]8/i,
        OSXMavericks: /os x 10[._]9/i,
        OSXYosemite: /os x 10[._]10/i,
        OSXElCapitan: /os x 10[._]11/i,
        OSXSierra: /os x 10[._]12/i,
        Mac: /os x/i,
        Linux: /linux/i,
        Linux64: /linux x86\_64/i,
        ChromeOS: /cros/i,
        Wii: /wii/i,
        PS3: /playstation 3/i,
        PSP: /playstation portable/i,
        iPad: /\(iPad.*os (\d+)[._](\d+)/i,
        iPhone: /\(iPhone.*os (\d+)[._](\d+)/i,
        Bada: /Bada\/(\d+)\.(\d+)/i,
        Curl: /curl\/(\d+)\.(\d+)\.(\d+)/i
    };
    this._Platform = {
        Windows: /windows nt/i,
        WindowsPhone: /windows phone/i,
        Mac: /macintosh/i,
        Linux: /linux/i,
        Wii: /wii/i,
        Playstation: /playstation/i,
        iPad: /ipad/i,
        iPod: /ipod/i,
        iPhone: /iphone/i,
        Android: /android/i,
        Blackberry: /blackberry/i,
        Samsung: /samsung/i,
        Curl: /curl/i
    };

    this.DefaultAgent = {
        isAuthoritative: true,
        isMobile: false,
        isTablet: false,
        isiPad: false,
        isiPod: false,
        isiPhone: false,
        isAndroid: false,
        isBlackberry: false,
        isOpera: false,
        isIE: false,
        isEdge: false,
        isIECompatibilityMode: false,
        isSafari: false,
        isFirefox: false,
        isWebkit: false,
        isChrome: false,
        isKonqueror: false,
        isOmniWeb: false,
        isSeaMonkey: false,
        isFlock: false,
        isAmaya: false,
        isPhantomJS: false,
        isEpiphany: false,
        isDesktop: false,
        isWindows: false,
        isLinux: false,
        isLinux64: false,
        isMac: false,
        isChromeOS: false,
        isBada: false,
        isSamsung: false,
        isRaspberry: false,
        isBot: false,
        isCurl: false,
        isAndroidTablet: false, ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-useragent.express"></a>[function <span class="apidocSignatureSpan">express-useragent.</span>express ()](#apidoc.element.express-useragent.express)
- description and source-code
```javascript
express = function () {
    return function (req, res, next) {
        var source = req.headers['user-agent'] || '';
        if (req.headers['x-ucbrowser-ua']) {  //special case of UC Browser
            source = req.headers['x-ucbrowser-ua'];
        }
        var ua = new UserAgent();
        if (typeof source === 'undefined') {
            source = "unknown";
        }
        ua.Agent.source = source.replace(/^\s*/, '').replace(/\s*$/, '');
        ua.Agent.os = ua.getOS(ua.Agent.source);
        ua.Agent.platform = ua.getPlatform(ua.Agent.source);
        ua.Agent.browser = ua.getBrowser(ua.Agent.source);
        ua.Agent.version = ua.getBrowserVersion(ua.Agent.source);
        ua.testNginxGeoIP(req.headers);
        ua.testBot();
        ua.testMobile();
        ua.testAndroidTablet();
        ua.testTablet();
        ua.testCompatibilityMode();
        ua.testSilk();
        ua.testKindleFire();
        req.useragent = ua.Agent;
        if ('function' === typeof res.locals) {
            res.locals({useragent: ua.Agent});
        } else {
            res.locals.useragent = ua.Agent;
        }
        next();
    };
}
```
- example usage
```shell
...
#### manual setup in project config/middleware.js

'''js
var useragent = require('express-useragent');

module.exports = function (app, express) {
    app.use(function () {
        app.use(useragent.express());
    });
};
'''

### for [ExpressJS](http://expressjs.com/)

'''js
...
```

#### <a name="apidoc.element.express-useragent.getBrowser"></a>[function <span class="apidocSignatureSpan">express-useragent.</span>getBrowser (string)](#apidoc.element.express-useragent.getBrowser)
- description and source-code
```javascript
getBrowser = function (string) {
    switch (true) {
        case this._Browsers.Edge.test(string):
            this.Agent.isEdge = true;
            return 'Edge';
        case this._Browsers.PhantomJS.test(string):
            this.Agent.isPhantomJS = true;
            return 'PhantomJS';
        case this._Browsers.Konqueror.test(string):
            this.Agent.isKonqueror = true;
            return 'Konqueror';
        case this._Browsers.Amaya.test(string):
            this.Agent.isAmaya = true;
            return 'Amaya';
        case this._Browsers.Epiphany.test(string):
            this.Agent.isEpiphany = true;
            return 'Epiphany';
        case this._Browsers.SeaMonkey.test(string):
            this.Agent.isSeaMonkey = true;
            return 'SeaMonkey';
        case this._Browsers.Flock.test(string):
            this.Agent.isFlock = true;
            return 'Flock';
        case this._Browsers.OmniWeb.test(string):
            this.Agent.isOmniWeb = true;
            return 'OmniWeb';
        case this._Browsers.Opera.test(string):
            this.Agent.isOpera = true;
            return 'Opera';
        case this._Browsers.Chromium.test(string):
            this.Agent.isChrome = true;
            return 'Chromium';
        case this._Browsers.Chrome.test(string):
            this.Agent.isChrome = true;
            return 'Chrome';
        case this._Browsers.WinJs.test(string):
            this.Agent.isWinJs = true;
            return 'WinJs';
        case this._Browsers.IE.test(string):
            this.Agent.isIE = true;
            return 'IE';
        case this._Browsers.Safari.test(string):
            this.Agent.isSafari = true;
            return 'Safari';
        case this._Browsers.PS3.test(string):
            return 'ps3';
        case this._Browsers.PSP.test(string):
            return 'psp';
        case this._Browsers.Firefox.test(string):
            this.Agent.isFirefox = true;
            return 'Firefox';
        case this._Browsers.UC.test(string):
            this.Agent.isUC = true;
            return 'UCBrowser';
        default:
            // If the UA does not start with Mozilla guess the user agent.
            if (string.indexOf('Mozilla') !== 0 && /^([\d\w\-\.]+)\/[\d\w\.\-]+/i.test(string)) {
                this.Agent.isAuthoritative = false;
                return RegExp.$1;
            }
            return 'unknown';
    }
}
```
- example usage
```shell
...
var ua = new UserAgent();
if (typeof source === 'undefined') {
    source = "unknown";
}
ua.Agent.source = source.replace(/^\s*/, '').replace(/\s*$/, '');
ua.Agent.os = ua.getOS(ua.Agent.source);
ua.Agent.platform = ua.getPlatform(ua.Agent.source);
ua.Agent.browser = ua.getBrowser(ua.Agent.source);
ua.Agent.version = ua.getBrowserVersion(ua.Agent.source);
ua.testNginxGeoIP(req.headers);
ua.testBot();
ua.testMobile();
ua.testAndroidTablet();
ua.testTablet();
ua.testCompatibilityMode();
...
```

#### <a name="apidoc.element.express-useragent.getBrowserVersion"></a>[function <span class="apidocSignatureSpan">express-useragent.</span>getBrowserVersion (string)](#apidoc.element.express-useragent.getBrowserVersion)
- description and source-code
```javascript
getBrowserVersion = function (string) {
    var regex;
    switch (this.Agent.browser) {
        case 'Edge':
            if (this._Versions.Edge.test(string)) {
                return RegExp.$1;
            }
            break;
        case 'PhantomJS':
            if (this._Versions.PhantomJS.test(string)) {
                return RegExp.$1;
            }
            break;
        case 'Chrome':
            if (this._Versions.Chrome.test(string)) {
                return RegExp.$1;
            }
            break;
        case 'Chromium':
            if (this._Versions.Chromium.test(string)) {
                return RegExp.$1;
            }
            break;
        case 'Safari':
            if (this._Versions.Safari.test(string)) {
                return RegExp.$1;
            }
            break;
        case 'Opera':
            if (this._Versions.Opera.test(string)) {
                return RegExp.$1 ? RegExp.$1: RegExp.$2;
            }
            break;
        case 'Firefox':
            if (this._Versions.Firefox.test(string)) {
                return RegExp.$1;
            }
            break;
        case 'WinJs':
            if (this._Versions.WinJs.test(string)) {
                return RegExp.$1;
            }
            break;
        case 'IE':
            if (this._Versions.IE.test(string)) {
                return RegExp.$2 ? RegExp.$2 : RegExp.$1;
            }
            break;
        case 'ps3':
            if (this._Versions.Ps3.test(string)) {
                return RegExp.$1;
            }
            break;
        case 'psp':
            if (this._Versions.Psp.test(string)) {
                return RegExp.$1;
            }
            break;
        case 'Amaya':
            if (this._Versions.Amaya.test(string)) {
                return RegExp.$1;
            }
            break;
        case 'Epiphany':
            if (this._Versions.Epiphany.test(string)) {
                return RegExp.$1;
            }
            break;
        case 'SeaMonkey':
            if (this._Versions.SeaMonkey.test(string)) {
                return RegExp.$1;
            }
            break;
        case 'Flock':
            if (this._Versions.Flock.test(string)) {
                return RegExp.$1;
            }
            break;
        case 'OmniWeb':
            if (this._Versions.OmniWeb.test(string)) {
                return RegExp.$1;
            }
            break;
        case 'UCBrowser':
            if (this._Versions.UC.test(string)) {
                return RegExp.$1;
            }
            break;
        default:
            if (this.Agent.browser !== 'unknown') {
                regex = new RegExp(this.Agent.browser + '[\\/ ]([\\d\\w\\.\\-]+)', 'i');
                if (regex.test(string)) {
                    return RegExp.$1;
                }
            }
    }
}
```
- example usage
```shell
...
if (typeof source === 'undefined') {
    source = "unknown";
}
ua.Agent.source = source.replace(/^\s*/, '').replace(/\s*$/, '');
ua.Agent.os = ua.getOS(ua.Agent.source);
ua.Agent.platform = ua.getPlatform(ua.Agent.source);
ua.Agent.browser = ua.getBrowser(ua.Agent.source);
ua.Agent.version = ua.getBrowserVersion(ua.Agent.source);
ua.testNginxGeoIP(req.headers);
ua.testBot();
ua.testMobile();
ua.testAndroidTablet();
ua.testTablet();
ua.testCompatibilityMode();
ua.testSilk();
...
```

#### <a name="apidoc.element.express-useragent.getOS"></a>[function <span class="apidocSignatureSpan">express-useragent.</span>getOS (string)](#apidoc.element.express-useragent.getOS)
- description and source-code
```javascript
getOS = function (string) {
    switch (true) {
        case this._OS.WindowsVista.test(string):
            this.Agent.isWindows = true;
            return 'Windows Vista';
        case this._OS.Windows7.test(string):
            this.Agent.isWindows = true;
            return 'Windows 7';
        case this._OS.Windows8.test(string):
            this.Agent.isWindows = true;
            return 'Windows 8';
        case this._OS.Windows81.test(string):
            this.Agent.isWindows = true;
            return 'Windows 8.1';
        case this._OS.Windows10.test(string):
            this.Agent.isWindows = true;
            return 'Windows 10.0';
        case this._OS.Windows2003.test(string):
            this.Agent.isWindows = true;
            return 'Windows 2003';
        case this._OS.WindowsXP.test(string):
            this.Agent.isWindows = true;
            return 'Windows XP';
        case this._OS.Windows2000.test(string):
            this.Agent.isWindows = true;
            return 'Windows 2000';
        case this._OS.WindowsPhone81.test(string):
            this.Agent.isWindowsPhone = true;
            return 'Windows Phone 8.1';
        case this._OS.WindowsPhone80.test(string):
            this.Agent.isWindowsPhone = true;
            return 'Windows Phone 8.0';
        case this._OS.Linux64.test(string):
            this.Agent.isLinux = true;
            this.Agent.isLinux64 = true;
            return 'Linux 64';
        case this._OS.Linux.test(string):
            this.Agent.isLinux = true;
            return 'Linux';
        case this._OS.ChromeOS.test(string):
            this.Agent.isChromeOS = true;
            return 'Chrome OS';
        case this._OS.Wii.test(string):
            return 'Wii';
        case this._OS.PS3.test(string):
            return 'Playstation';
        case this._OS.PSP.test(string):
            return 'Playstation';
        case this._OS.OSXCheetah.test(string):
            this.Agent.isMac = true;
            return 'OS X Cheetah';
        case this._OS.OSXPuma.test(string):
            this.Agent.isMac = true;
            return 'OS X Puma';
        case this._OS.OSXJaguar.test(string):
            this.Agent.isMac = true;
            return 'OS X Jaguar';
        case this._OS.OSXPanther.test(string):
            this.Agent.isMac = true;
            return 'OS X Panther';
        case this._OS.OSXTiger.test(string):
            this.Agent.isMac = true;
            return 'OS X Tiger';
        case this._OS.OSXLeopard.test(string):
            this.Agent.isMac = true;
            return 'OS X Leopard';
        case this._OS.OSXSnowLeopard.test(string):
            this.Agent.isMac = true;
            return 'OS X Snow Leopard';
        case this._OS.OSXLion.test(string):
            this.Agent.isMac = true;
            return 'OS X Lion';
        case this._OS.OSXMountainLion.test(string):
            this.Agent.isMac = true;
            return 'OS X Mountain Lion';
        case this._OS.OSXMavericks.test(string):
            this.Agent.isMac = true;
            return 'OS X Mavericks';
        case this._OS.OSXYosemite.test(string):
            this.Agent.isMac = true;
            return 'OS X Yosemite';
        case this._OS.OSXElCapitan.test(string):
            this.Agent.isMac = true;
            return 'OS X El Capitan';
        case this._OS.OSXSierra.test(string):
            this.Agent.isMac = true;
            return 'macOS Sierra';
        case this._OS.Mac.test(string):
            this.Agent.isMac = true;
            return 'OS X';
        case this._OS.iPad.test(string):
            this.Agent.isiPad = true;
            return string.match(this._OS.iPad)[0].replace('_', '.');
        case this._OS.iPhone.test(string):
            this.Agent.isiPhone = true;
            return string.match(this._OS.iPhone)[0].replace('_', '.');
        case this._OS.Bada.test(string):
            this.Agent.isBada = true;
            return 'Bada';
        case this._OS.Curl.test(string):
            this.Agent.isCurl = true;
            return 'Curl';
        default:
            return ...
```
- example usage
```shell
...
    source = req.headers['x-ucbrowser-ua'];
}
var ua = new UserAgent();
if (typeof source === 'undefined') {
    source = "unknown";
}
ua.Agent.source = source.replace(/^\s*/, '').replace(/\s*$/, '');
ua.Agent.os = ua.getOS(ua.Agent.source);
ua.Agent.platform = ua.getPlatform(ua.Agent.source);
ua.Agent.browser = ua.getBrowser(ua.Agent.source);
ua.Agent.version = ua.getBrowserVersion(ua.Agent.source);
ua.testNginxGeoIP(req.headers);
ua.testBot();
ua.testMobile();
ua.testAndroidTablet();
...
```

#### <a name="apidoc.element.express-useragent.getPlatform"></a>[function <span class="apidocSignatureSpan">express-useragent.</span>getPlatform (string)](#apidoc.element.express-useragent.getPlatform)
- description and source-code
```javascript
getPlatform = function (string) {
    switch (true) {
        case this._Platform.Windows.test(string):
            return 'Microsoft Windows';
        case this._Platform.WindowsPhone.test(string):
            this.Agent.isWindowsPhone = true;
            return 'Microsoft Windows Phone';
        case this._Platform.Mac.test(string):
            return 'Apple Mac';
        case this._Platform.Curl.test(string):
            return 'Curl';
        case this._Platform.Android.test(string):
            this.Agent.isAndroid = true;
            return 'Android';
        case this._Platform.Blackberry.test(string):
            this.Agent.isBlackberry = true;
            return 'Blackberry';
        case this._Platform.Linux.test(string):
            return 'Linux';
        case this._Platform.Wii.test(string):
            return 'Wii';
        case this._Platform.Playstation.test(string):
            return 'Playstation';
        case this._Platform.iPad.test(string):
            this.Agent.isiPad = true;
            return 'iPad';
        case this._Platform.iPod.test(string):
            this.Agent.isiPod = true;
            return 'iPod';
        case this._Platform.iPhone.test(string):
            this.Agent.isiPhone = true;
            return 'iPhone';
        case this._Platform.Samsung.test(string):
            this.Agent.isiSamsung = true;
            return 'Samsung';
        default:
            return 'unknown';
    }
}
```
- example usage
```shell
...
}
var ua = new UserAgent();
if (typeof source === 'undefined') {
    source = "unknown";
}
ua.Agent.source = source.replace(/^\s*/, '').replace(/\s*$/, '');
ua.Agent.os = ua.getOS(ua.Agent.source);
ua.Agent.platform = ua.getPlatform(ua.Agent.source);
ua.Agent.browser = ua.getBrowser(ua.Agent.source);
ua.Agent.version = ua.getBrowserVersion(ua.Agent.source);
ua.testNginxGeoIP(req.headers);
ua.testBot();
ua.testMobile();
ua.testAndroidTablet();
ua.testTablet();
...
```

#### <a name="apidoc.element.express-useragent.parse"></a>[function <span class="apidocSignatureSpan">express-useragent.</span>parse (source)](#apidoc.element.express-useragent.parse)
- description and source-code
```javascript
function parse(source) {
    var ua = new UserAgent();
    ua.Agent.source = source.replace(/^\s*/, '').replace(/\s*$/, '');
    ua.Agent.os = ua.getOS(ua.Agent.source);
    ua.Agent.platform = ua.getPlatform(ua.Agent.source);
    ua.Agent.browser = ua.getBrowser(ua.Agent.source);
    ua.Agent.version = ua.getBrowserVersion(ua.Agent.source);
    ua.testBot();
    ua.testSmartTV();
    ua.testMobile();
    ua.testAndroidTablet();
    ua.testTablet();
    ua.testCompatibilityMode();
    ua.testSilk();
    ua.testKindleFire();
    ua.testCaptiveNetwork();
    return ua.Agent;
}
```
- example usage
```shell
...

'''js
var http = require('http')
  , useragent = require('express-useragent');

var srv = http.createServer(function (req, res) {
  var source = req.headers['user-agent'],
  ua = useragent.parse(source);
  res.writeHead(200, {'Content-Type': 'text/plain'});
  res.end(JSON.stringify(ua));
});

srv.listen(3000);
'''
...
```

#### <a name="apidoc.element.express-useragent.reset"></a>[function <span class="apidocSignatureSpan">express-useragent.</span>reset ()](#apidoc.element.express-useragent.reset)
- description and source-code
```javascript
function reset() {
    var ua = this;
    for (var key in ua.DefaultAgent) {
        ua.Agent[key] = ua.DefaultAgent[key];
    }
    return ua;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-useragent.testAndroidTablet"></a>[function <span class="apidocSignatureSpan">express-useragent.</span>testAndroidTablet ()](#apidoc.element.express-useragent.testAndroidTablet)
- description and source-code
```javascript
function testAndroidTablet() {
    var ua = this;
    if (ua.Agent.isAndroid && !/mobile/i.test(ua.Agent.source)) {
        ua.Agent.isAndroidTablet = true;
    }
}
```
- example usage
```shell
...
ua.Agent.os = ua.getOS(ua.Agent.source);
ua.Agent.platform = ua.getPlatform(ua.Agent.source);
ua.Agent.browser = ua.getBrowser(ua.Agent.source);
ua.Agent.version = ua.getBrowserVersion(ua.Agent.source);
ua.testNginxGeoIP(req.headers);
ua.testBot();
ua.testMobile();
ua.testAndroidTablet();
ua.testTablet();
ua.testCompatibilityMode();
ua.testSilk();
ua.testKindleFire();
req.useragent = ua.Agent;
if ('function' === typeof res.locals) {
    res.locals({useragent: ua.Agent});
...
```

#### <a name="apidoc.element.express-useragent.testBot"></a>[function <span class="apidocSignatureSpan">express-useragent.</span>testBot ()](#apidoc.element.express-useragent.testBot)
- description and source-code
```javascript
function testBot() {
    var ua = this;
    var isBot = IS_BOT_REGEXP.exec(ua.Agent.source.toLowerCase());
    if (isBot) {
        ua.Agent.isBot = isBot[1];
    } else if (!ua.Agent.isAuthoritative) {
        // Test unauthoritative parse for 'bot' in UA to flag for bot
        ua.Agent.isBot = /bot/i.test(ua.Agent.source);
    }
}
```
- example usage
```shell
...
}
ua.Agent.source = source.replace(/^\s*/, '').replace(/\s*$/, '');
ua.Agent.os = ua.getOS(ua.Agent.source);
ua.Agent.platform = ua.getPlatform(ua.Agent.source);
ua.Agent.browser = ua.getBrowser(ua.Agent.source);
ua.Agent.version = ua.getBrowserVersion(ua.Agent.source);
ua.testNginxGeoIP(req.headers);
ua.testBot();
ua.testMobile();
ua.testAndroidTablet();
ua.testTablet();
ua.testCompatibilityMode();
ua.testSilk();
ua.testKindleFire();
req.useragent = ua.Agent;
...
```

#### <a name="apidoc.element.express-useragent.testCaptiveNetwork"></a>[function <span class="apidocSignatureSpan">express-useragent.</span>testCaptiveNetwork ()](#apidoc.element.express-useragent.testCaptiveNetwork)
- description and source-code
```javascript
testCaptiveNetwork = function () {
    var ua = this;
    switch (true) {
        case /CaptiveNetwork/gi.test(ua.Agent.source):
            ua.Agent.isCaptive = true;
            ua.Agent.isMac = true;
            ua.Agent.platform = 'Apple Mac';
            return 'CaptiveNetwork';
        default:
            return false;
    }
}
```
- example usage
```shell
...
        ua.testSmartTV();
        ua.testMobile();
        ua.testAndroidTablet();
        ua.testTablet();
        ua.testCompatibilityMode();
        ua.testSilk();
        ua.testKindleFire();
        ua.testCaptiveNetwork();
        return ua.Agent;
    };

    this.Agent = this.DefaultAgent;
    return this;
};
...
```

#### <a name="apidoc.element.express-useragent.testCompatibilityMode"></a>[function <span class="apidocSignatureSpan">express-useragent.</span>testCompatibilityMode ()](#apidoc.element.express-useragent.testCompatibilityMode)
- description and source-code
```javascript
testCompatibilityMode = function () {
    var ua = this;
    if (this.Agent.isIE) {
        if (/Trident\/(\d)\.0/i.test(ua.Agent.source)) {
            var tridentVersion = parseInt(RegExp.$1, 10);
            var version = parseInt(ua.Agent.version, 10);
            if (version === 7 && tridentVersion === 7) {
                ua.Agent.isIECompatibilityMode = true;
                ua.Agent.version = 11.0;
            }

            if (version === 7 && tridentVersion === 6) {
                ua.Agent.isIECompatibilityMode = true;
                ua.Agent.version = 10.0;
            }

            if (version === 7 && tridentVersion === 5) {
                ua.Agent.isIECompatibilityMode = true;
                ua.Agent.version = 9.0;
            }

            if (version === 7 && tridentVersion === 4) {
                ua.Agent.isIECompatibilityMode = true;
                ua.Agent.version = 8.0;
            }
        }
    }
}
```
- example usage
```shell
...
ua.Agent.browser = ua.getBrowser(ua.Agent.source);
ua.Agent.version = ua.getBrowserVersion(ua.Agent.source);
ua.testNginxGeoIP(req.headers);
ua.testBot();
ua.testMobile();
ua.testAndroidTablet();
ua.testTablet();
ua.testCompatibilityMode();
ua.testSilk();
ua.testKindleFire();
req.useragent = ua.Agent;
if ('function' === typeof res.locals) {
    res.locals({useragent: ua.Agent});
} else {
    res.locals.useragent = ua.Agent;
...
```

#### <a name="apidoc.element.express-useragent.testKindleFire"></a>[function <span class="apidocSignatureSpan">express-useragent.</span>testKindleFire ()](#apidoc.element.express-useragent.testKindleFire)
- description and source-code
```javascript
testKindleFire = function () {
    var ua = this;
    switch (true) {
        case /KFOT/gi.test(ua.Agent.source):
            this.Agent.isKindleFire = true;
            return 'Kindle Fire';
        case /KFTT/gi.test(ua.Agent.source):
            this.Agent.isKindleFire = true;
            return 'Kindle Fire HD';
        case /KFJWI/gi.test(ua.Agent.source):
            this.Agent.isKindleFire = true;
            return 'Kindle Fire HD 8.9';
        case /KFJWA/gi.test(ua.Agent.source):
            this.Agent.isKindleFire = true;
            return 'Kindle Fire HD 8.9 4G';
        case /KFSOWI/gi.test(ua.Agent.source):
            this.Agent.isKindleFire = true;
            return 'Kindle Fire HD 7';
        case /KFTHWI/gi.test(ua.Agent.source):
            this.Agent.isKindleFire = true;
            return 'Kindle Fire HDX 7';
        case /KFTHWA/gi.test(ua.Agent.source):
            this.Agent.isKindleFire = true;
            return 'Kindle Fire HDX 7 4G';
        case /KFAPWI/gi.test(ua.Agent.source):
            this.Agent.isKindleFire = true;
            return 'Kindle Fire HDX 8.9';
        case /KFAPWA/gi.test(ua.Agent.source):
            this.Agent.isKindleFire = true;
            return 'Kindle Fire HDX 8.9 4G';
        default:
            return false;
    }
}
```
- example usage
```shell
...
ua.testNginxGeoIP(req.headers);
ua.testBot();
ua.testMobile();
ua.testAndroidTablet();
ua.testTablet();
ua.testCompatibilityMode();
ua.testSilk();
ua.testKindleFire();
req.useragent = ua.Agent;
if ('function' === typeof res.locals) {
    res.locals({useragent: ua.Agent});
} else {
    res.locals.useragent = ua.Agent;
}
next();
...
```

#### <a name="apidoc.element.express-useragent.testMobile"></a>[function <span class="apidocSignatureSpan">express-useragent.</span>testMobile ()](#apidoc.element.express-useragent.testMobile)
- description and source-code
```javascript
function testMobile() {
    var ua = this;
    switch (true) {
        case ua.Agent.isWindows:
        case ua.Agent.isLinux:
        case ua.Agent.isMac:
        case ua.Agent.isChromeOS:
            ua.Agent.isDesktop = true;
            break;
        case ua.Agent.isAndroid:
        case ua.Agent.isSamsung:
            ua.Agent.isMobile = true;
            ua.Agent.isDesktop = false;
            break;
        default:
    }
    switch (true) {
        case ua.Agent.isiPad:
        case ua.Agent.isiPod:
        case ua.Agent.isiPhone:
        case ua.Agent.isBada:
        case ua.Agent.isBlackberry:
        case ua.Agent.isAndroid:
        case ua.Agent.isWindowsPhone:
            ua.Agent.isMobile = true;
            ua.Agent.isDesktop = false;
            break;
        default:
    }
    if (/mobile/i.test(ua.Agent.source)) {
        ua.Agent.isMobile = true;
        ua.Agent.isDesktop = false;
    }
}
```
- example usage
```shell
...
ua.Agent.source = source.replace(/^\s*/, '').replace(/\s*$/, '');
ua.Agent.os = ua.getOS(ua.Agent.source);
ua.Agent.platform = ua.getPlatform(ua.Agent.source);
ua.Agent.browser = ua.getBrowser(ua.Agent.source);
ua.Agent.version = ua.getBrowserVersion(ua.Agent.source);
ua.testNginxGeoIP(req.headers);
ua.testBot();
ua.testMobile();
ua.testAndroidTablet();
ua.testTablet();
ua.testCompatibilityMode();
ua.testSilk();
ua.testKindleFire();
req.useragent = ua.Agent;
if ('function' === typeof res.locals) {
...
```

#### <a name="apidoc.element.express-useragent.testNginxGeoIP"></a>[function <span class="apidocSignatureSpan">express-useragent.</span>testNginxGeoIP (headers)](#apidoc.element.express-useragent.testNginxGeoIP)
- description and source-code
```javascript
function testNginxGeoIP(headers) {
    var ua = this;
    Object.keys(headers).forEach(function (key) {
        if (/^GEOIP/i.test(key)) {
            ua.Agent.geoIp[key] = headers[key];
        }
    });
}
```
- example usage
```shell
...
    source = "unknown";
}
ua.Agent.source = source.replace(/^\s*/, '').replace(/\s*$/, '');
ua.Agent.os = ua.getOS(ua.Agent.source);
ua.Agent.platform = ua.getPlatform(ua.Agent.source);
ua.Agent.browser = ua.getBrowser(ua.Agent.source);
ua.Agent.version = ua.getBrowserVersion(ua.Agent.source);
ua.testNginxGeoIP(req.headers);
ua.testBot();
ua.testMobile();
ua.testAndroidTablet();
ua.testTablet();
ua.testCompatibilityMode();
ua.testSilk();
ua.testKindleFire();
...
```

#### <a name="apidoc.element.express-useragent.testSilk"></a>[function <span class="apidocSignatureSpan">express-useragent.</span>testSilk ()](#apidoc.element.express-useragent.testSilk)
- description and source-code
```javascript
testSilk = function () {
    var ua = this;
    switch (true) {
        case new RegExp('silk', 'gi').test(ua.Agent.source):
            this.Agent.isSilk = true;
            break;
        default:
    }

    if (/Silk-Accelerated=true/gi.test(ua.Agent.source)) {
    this.Agent.SilkAccelerated = true;
    }
    return this.Agent.isSilk ? 'Silk' : false;
}
```
- example usage
```shell
...
ua.Agent.version = ua.getBrowserVersion(ua.Agent.source);
ua.testNginxGeoIP(req.headers);
ua.testBot();
ua.testMobile();
ua.testAndroidTablet();
ua.testTablet();
ua.testCompatibilityMode();
ua.testSilk();
ua.testKindleFire();
req.useragent = ua.Agent;
if ('function' === typeof res.locals) {
    res.locals({useragent: ua.Agent});
} else {
    res.locals.useragent = ua.Agent;
}
...
```

#### <a name="apidoc.element.express-useragent.testSmartTV"></a>[function <span class="apidocSignatureSpan">express-useragent.</span>testSmartTV ()](#apidoc.element.express-useragent.testSmartTV)
- description and source-code
```javascript
function testBot() {
    var ua = this;
    var isSmartTV = new RegExp('smart-tv|smarttv|googletv|appletv|hbbtv|pov_tv|netcast.tv','gi').exec(ua.Agent.source.toLowerCase
());
    if (isSmartTV) {
        ua.Agent.isSmartTV = isSmartTV[1];
    }
}
```
- example usage
```shell
...
var ua = new UserAgent();
ua.Agent.source = source.replace(/^\s*/, '').replace(/\s*$/, '');
ua.Agent.os = ua.getOS(ua.Agent.source);
ua.Agent.platform = ua.getPlatform(ua.Agent.source);
ua.Agent.browser = ua.getBrowser(ua.Agent.source);
ua.Agent.version = ua.getBrowserVersion(ua.Agent.source);
ua.testBot();
ua.testSmartTV();
ua.testMobile();
ua.testAndroidTablet();
ua.testTablet();
ua.testCompatibilityMode();
ua.testSilk();
ua.testKindleFire();
ua.testCaptiveNetwork();
...
```

#### <a name="apidoc.element.express-useragent.testTablet"></a>[function <span class="apidocSignatureSpan">express-useragent.</span>testTablet ()](#apidoc.element.express-useragent.testTablet)
- description and source-code
```javascript
function testTablet() {
    var ua = this;
    switch (true) {
        case ua.Agent.isiPad:
        case ua.Agent.isAndroidTablet:
        case ua.Agent.isKindleFire:
            ua.Agent.isTablet = true;
            break;
    }
    if (/tablet/i.test(ua.Agent.source)) {
        ua.Agent.isTablet = true;
    }
}
```
- example usage
```shell
...
ua.Agent.platform = ua.getPlatform(ua.Agent.source);
ua.Agent.browser = ua.getBrowser(ua.Agent.source);
ua.Agent.version = ua.getBrowserVersion(ua.Agent.source);
ua.testNginxGeoIP(req.headers);
ua.testBot();
ua.testMobile();
ua.testAndroidTablet();
ua.testTablet();
ua.testCompatibilityMode();
ua.testSilk();
ua.testKindleFire();
req.useragent = ua.Agent;
if ('function' === typeof res.locals) {
    res.locals({useragent: ua.Agent});
} else {
...
```



# <a name="apidoc.module.express-useragent.express_useragent"></a>[module express-useragent.express_useragent](#apidoc.module.express-useragent.express_useragent)

#### <a name="apidoc.element.express-useragent.express_useragent.UserAgent"></a>[function <span class="apidocSignatureSpan">express-useragent.express_useragent.</span>UserAgent ()](#apidoc.element.express-useragent.express_useragent.UserAgent)
- description and source-code
```javascript
UserAgent = function () {
    this.version = '1.0.4';
    this._Versions = {
        Edge: /Edge\/([\d\w\.\-]+)/i,
        Firefox: /firefox\/([\d\w\.\-]+)/i,
        IE: /msie\s([\d\.]+[\d])|trident\/\d+\.\d+;.*[rv:]+(\d+\.\d)/i,
        Chrome: /chrome\/([\d\w\.\-]+)/i,
        Chromium: /(?:chromium|crios)\/([\d\w\.\-]+)/i,
        Safari: /version\/([\d\w\.\-]+)/i,
        Opera: /version\/([\d\w\.\-]+)|OPR\/([\d\w\.\-]+)/i,
        Ps3: /([\d\w\.\-]+)\)\s*$/i,
        Psp: /([\d\w\.\-]+)\)?\s*$/i,
        Amaya: /amaya\/([\d\w\.\-]+)/i,
        SeaMonkey: /seamonkey\/([\d\w\.\-]+)/i,
        OmniWeb: /omniweb\/v([\d\w\.\-]+)/i,
        Flock: /flock\/([\d\w\.\-]+)/i,
        Epiphany: /epiphany\/([\d\w\.\-]+)/i,
        WinJs: /msapphost\/([\d\w\.\-]+)/i,
        PhantomJS: /phantomjs\/([\d\w\.\-]+)/i,
        UC: /UCBrowser\/([\d\w\.]+)/i
    };
    this._Browsers = {
        Edge: /edge/i,
        Amaya: /amaya/i,
        Konqueror: /konqueror/i,
        Epiphany: /epiphany/i,
        SeaMonkey: /seamonkey/i,
        Flock: /flock/i,
        OmniWeb: /omniweb/i,
        Chromium: /chromium|crios/i,
        Chrome: /chrome/i,
        Safari: /safari/i,
        IE: /msie|trident/i,
        Opera: /opera|OPR/i,
        PS3: /playstation 3/i,
        PSP: /playstation portable/i,
        Firefox: /firefox/i,
        WinJs: /msapphost/i,
        PhantomJS: /phantomjs/i,
        UC: /UCBrowser/i
    };
    this._OS = {
        Windows10: /windows nt 10\.0/i,
        Windows81: /windows nt 6\.3/i,
        Windows8: /windows nt 6\.2/i,
        Windows7: /windows nt 6\.1/i,
        UnknownWindows: /windows nt 6\.\d+/i,
        WindowsVista: /windows nt 6\.0/i,
        Windows2003: /windows nt 5\.2/i,
        WindowsXP: /windows nt 5\.1/i,
        Windows2000: /windows nt 5\.0/i,
        WindowsPhone81: /windows phone 8\.1/i,
        WindowsPhone80: /windows phone 8\.0/i,
        OSXCheetah: /os x 10[._]0/i,
        OSXPuma: /os x 10[._]1(\D|$)/i,
        OSXJaguar: /os x 10[._]2/i,
        OSXPanther: /os x 10[._]3/i,
        OSXTiger: /os x 10[._]4/i,
        OSXLeopard: /os x 10[._]5/i,
        OSXSnowLeopard: /os x 10[._]6/i,
        OSXLion: /os x 10[._]7/i,
        OSXMountainLion: /os x 10[._]8/i,
        OSXMavericks: /os x 10[._]9/i,
        OSXYosemite: /os x 10[._]10/i,
        OSXElCapitan: /os x 10[._]11/i,
        OSXSierra: /os x 10[._]12/i,
        Mac: /os x/i,
        Linux: /linux/i,
        Linux64: /linux x86\_64/i,
        ChromeOS: /cros/i,
        Wii: /wii/i,
        PS3: /playstation 3/i,
        PSP: /playstation portable/i,
        iPad: /\(iPad.*os (\d+)[._](\d+)/i,
        iPhone: /\(iPhone.*os (\d+)[._](\d+)/i,
        Bada: /Bada\/(\d+)\.(\d+)/i,
        Curl: /curl\/(\d+)\.(\d+)\.(\d+)/i
    };
    this._Platform = {
        Windows: /windows nt/i,
        WindowsPhone: /windows phone/i,
        Mac: /macintosh/i,
        Linux: /linux/i,
        Wii: /wii/i,
        Playstation: /playstation/i,
        iPad: /ipad/i,
        iPod: /ipod/i,
        iPhone: /iphone/i,
        Android: /android/i,
        Blackberry: /blackberry/i,
        Samsung: /samsung/i,
        Curl: /curl/i
    };

    this.DefaultAgent = {
        isAuthoritative: true,
        isMobile: false,
        isTablet: false,
        isiPad: false,
        isiPod: false,
        isiPhone: false,
        isAndroid: false,
        isBlackberry: false,
        isOpera: false,
        isIE: false,
        isEdge: false,
        isIECompatibilityMode: false,
        isSafari: false,
        isFirefox: false,
        isWebkit: false,
        isChrome: false,
        isKonqueror: false,
        isOmniWeb: false,
        isSeaMonkey: false,
        isFlock: false,
        isAmaya: false,
        isPhantomJS: false,
        isEpiphany: false,
        isDesktop: false,
        isWindows: false,
        isLinux: false,
        isLinux64: false,
        isMac: false,
        isChromeOS: false,
        isBada: false,
        isSamsung: false,
        isRaspberry: false,
        isBot: false,
        isCurl: false,
        isAndroidTablet: false, ...
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
