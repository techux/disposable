# 🗑 Disposable email domains

[![npm](https://badge.fury.io/js/disposable-email.svg)](https://www.npmjs.com/package/disposable-email)
[![GoDoc](https://godoc.org/github.com/disposable/disposable?status.svg)](https://godoc.org/github.com/disposable/disposable)

A collection of domains for disposable email services like [10MinuteMail](http://10minutemail.com) and [GuerrillaMail](https://www.guerrillamail.com). Also, some 🛠 to make your life easier.

## Why?

Use it to validate email addresses on sign up, or just to see how many real email addresses you have in your system.

## Usage

### List

A [file](https://raw.githubusercontent.com/disposable/disposable-email-domains/master/domains.txt)
containing a sorted list of domains, one per line.

```shell
curl https://raw.githubusercontent.com/disposable/disposable-email-domains/master/domains.txt
```

### JSON array

A [file](https://raw.githubusercontent.com/disposable/disposable-email-domains/master/domains.json)
containing a sorted array of domains, in JSON format.

```shell
curl https://raw.githubusercontent.com/disposable/disposable-email-domains/master/domains.json
```

### JavaScript

Install the npm package `disposable-email`. Validate synchronously or with a callback.

```shell
npm i --save disposable-email
```

```javascript
var disposable = require('disposable-email');

disposable.validate('gmail.com');
// true

disposable.validate('foo@gmail.com');
// true

disposable.validate('gmail.com', console.log);
// undefined
// null true
```

### Go

```go
import "github.com/disposable/disposable"

if disposable.Domain("gmail.com") {
    panic("Uh oh!")
}
```

## Update the list of domains

To update the list of domains run `.generate` (requires `python3`), and optionally submit a PR.

```shell
$ ./.generate
Fetched 5196 domains and 6593 hashes
 - 2000 domain(s) added
 - 75 domain(s) removed
 - 2010 hash(es) added
 - 76 hash(es) removed
```

## External Sources:
|Source|Status|
|------|--:|
|https://gist.github.com/adamloving/4401361/|![GitHub last update](https://img.shields.io/badge/dynamic/json?color=lightgray&style=flat&label=last%20update&query=%24.updated_at&url=https%3A%2F%2Fapi.github.com%2Fgists%2F4401361&cacheSeconds=3600)|
|https://gist.github.com/michenriksen/8710649/|![GitHub last update](https://img.shields.io/badge/dynamic/json?color=lightgray&style=flat&label=last%20update&query=%24.updated_at&url=https%3A%2F%2Fapi.github.com%2Fgists%2F8710649&cacheSeconds=3600)|
|https://gist.github.com/jamesonev/7e188c35fd5ca754c970e3a1caf045ef/|![GitHub last update](https://img.shields.io/badge/dynamic/json?color=lightgray&style=flat&label=last%20update&query=%24.updated_at&url=https%3A%2F%2Fapi.github.com%2Fgists%2F7e188c35fd5ca754c970e3a1caf045ef&cacheSeconds=3600)|
|https://github.com/disposable/static-disposable-lists/|![GitHub last commit](https://img.shields.io/github/last-commit/disposable/static-disposable-lists)|
|https://github.com/wesbos/burner-email-providers/|![GitHub last commit](https://img.shields.io/github/last-commit/wesbos/burner-email-providers)|
|https://github.com/GeroldSetz/emailondeck.com-domains/| ![GitHub last commit](https://img.shields.io/github/last-commit/GeroldSetz/emailondeck.com-domains) |
|https://github.com/willwhite/freemail/|![GitHub last commit](https://img.shields.io/github/last-commit/willwhite/freemail)|
|https://github.com/stopforumspam/disposable_email_domains/|![GitHub last commit](https://img.shields.io/github/last-commit/stopforumspam/disposable_email_domains)|
|https://github.com/martenson/disposable-email-domains/|![GitHub last commit](https://img.shields.io/github/last-commit/martenson/disposable-email-domains)|
|https://github.com/daisy1754/jp-disposable-emails/|![GitHub last commit](https://img.shields.io/github/last-commit/daisy1754/jp-disposable-emails)|
|https://github.com/FGRibreau/mailchecker/|![GitHub last commit](https://img.shields.io/github/last-commit/FGRibreau/mailchecker)|
|https://github.com/ivolo/disposable-email-domains/|![GitHub last commit](https://img.shields.io/github/last-commit/ivolo/disposable-email-domains)|


## Credits

[@adamloving](https://github.com/adamloving)
[@michenriksen](https://github.com/michenriksen)
[@ivolo](https://github.com/ivolo)
[@smeinecke](https://github.com/smeinecke)
[@GeroldSetz](https://github.com/GeroldSetz)
[@martenson](https://github.com/martenson)
[@FGRibreau](https://github.com/FGRibreau)
[@daisy1754](https://github.com/daisy1754)
[@jamesonev](https://github.com/jamesonev)
[@wesbos](https://github.com/wesbos)
[@willwhite](https://github.com/willwhite)
[@stopforumspam](https://github.com/stopforumspam)

### CDN

* Production: https://rawcdn.githack.com/disposable/disposable-email-domains/master/domains.json
* Development: https://raw.githack.com/disposable/disposable-email-domains/master/domains.json

by: https://raw.githack.com/
