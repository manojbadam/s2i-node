
```
docker build -t base-nodejs .
s2i build https://github.com/debianmaster/nodejs-welcome.git manoj-nodejs hello-nodejs
```