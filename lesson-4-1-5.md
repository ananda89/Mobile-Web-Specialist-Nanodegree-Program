# Client-Server Communication

## HTTP's Request/Response Cycle

* Common abbreviations:
   * __SGML__ - Standard Generalized Markup Language
   * __HTML__ - HyperText Markup Language
   * __HTTP__ - Hypertext Transfer Protocol


* Example of HTTP request:

```
GET /sebastianczech/Mobile-Web-Specialist-Nanodegree-Program HTTP/1.1
Host: github.com
Connection: keep-alive
Cache-Control: max-age=0
Upgrade-Insecure-Requests: 1
User-Agent: Mozilla/5.0 (Macintosh; Intel Mac OS X 10_13_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/65.0.3325.181 Safari/537.36
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8
Referer: https://github.com/sebastianczech
Accept-Encoding: gzip, deflate, br
Accept-Language: pl-PL,pl;q=0.9,en-US;q=0.8,en;q=0.7,de;q=0.6
```


* Example of HTTP response:

```
HTTP/1.1 200 OK
Server: GitHub.com
Date: Thu, 05 Apr 2018 21:17:49 GMT
Content-Type: text/html; charset=utf-8
Transfer-Encoding: chunked
Status: 200 OK
X-Frame-Options: deny
X-XSS-Protection: 1; mode=block
X-Content-Type-Options: nosniff
Cache-Control: no-cache
Vary: X-PJAX
X-Request-Id: ffab99b4-bd70-45b3-9bb5-11f9be6e7eda
X-Runtime: 0.290211
Strict-Transport-Security: max-age=31536000; includeSubdomains; preload
Expect-CT: max-age=2592000, report-uri="https://api.github.com/_private/browser/errors"
X-Runtime-rack: 0.296850
Content-Encoding: gzip
X-GitHub-Request-Id: E324:5AF5:6956FA:C58636:5AC69276
...
```


* Useful links:
   * [Introduction to fetch()](https://developers.google.com/web/updates/2015/03/introduction-to-fetch?hl=en)
   * [That's so fetch!](https://jakearchibald.com/2015/thats-so-fetch/)
   * [JavaScript Promises: an Introduction](https://developers.google.com/web/fundamentals/primers/promises?hl=en)
   * [Using Fetch](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch)

## HTTP/1

* Useful links:
   * [Netcat - TCP/IP swiss Army](http://nc110.sourceforge.net/)
   * [Netcat (nc)](https://en.wikipedia.org/wiki/Netcat)
   * [HTTP request methods](https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods)
   * [HTTP header fields](https://en.wikipedia.org/wiki/List_of_HTTP_header_fields)
   * [REST API tutorial](http://www.restapitutorial.com/)

## HTTPS

* Common abbreviations:
   * __TLS__ - Transport Layer Security


* TLS -> encryption + hashing   


* Useful links:
   * [Firesheep](http://codebutler.com/firesheep)
   * [Man in the middle attack (MITM)](https://en.wikipedia.org/wiki/Man-in-the-middle_attack)
   * [Let's Encrypt - Free SSL/TLS Certificates](https://letsencrypt.org/)
   * [Bad SSL](https://badssl.com/)
   * [Mixed content](https://developer.mozilla.org/en-US/docs/Web/Security/Mixed_content)

## HTTP/2

* HTTP/1 problems:
   * __HOL__ - head-of-line blocking (resolved in HTTP/2 by multiplexing and sharing connection)
   * uncompressed headers
   * security (resolved in HTTP/2 by TLS)

* Round trip = request + response

* Useful links:
   * [Report: State of the Web ](https://httparchive.org/reports/state-of-the-web)
   * [SPDY: An experimental protocol for a faster web](http://dev.chromium.org/spdy/spdy-whitepaper)
   * [gzip in HTML5 Boilerplate project](https://github.com/h5bp/html5-boilerplate/blob/master/dist/.htaccess#L709-L795)
   * [HPACK: Header Compression for HTTP/2](https://http2.github.io/http2-spec/compression.html)
   * [Can I use HTTP/2 protocol](https://caniuse.com/#feat=http2)

## Security

* Origin = Data Scheme + Hostname + Port e.g. ``https://`` + ``www.google.com`` + ``:443``

* Cross-Origin Fetch Requests are not allowed

* __CORS__ - Cross Origin Resource Sharing

* _Message passing_ - technique designed to allow cross-origin communication. ```postMessage()``` is a function to pass a message to other windows and iframes, even if they come from a different origin.

* __JSONP__ - JSON with padding

* __CSRF__ - Cross-site request forgery

* __XSS__ - Cross-site scripting

* Useful links:
   * [Same Origin Policy](https://www.w3.org/Security/wiki/Same_Origin_Policy)
   * [Cross-Origin Resource Sharing (CORS)](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS)
   * [Cross-site scripting (XSS)](https://en.wikipedia.org/wiki/Cross-site_scripting)
