
```
docker build -t base-nodejs .
s2i build https://github.com/debianmaster/nodejs-welcome.git base-nodejs hello-nodejs
```
