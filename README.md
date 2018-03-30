
This is a sample project using [source-to-image](https://github.com/openshift/source-to-image) to build the template base image.

## Setup
Please install the latest s2i (source-to-image) binary from [here](https://github.com/openshift/source-to-image#installation)
Once the s2i binary is installed, check if it is properly configured in your path `s2i version`

```
git clone git@github.com:manojbadam/s2i-node.git
cd s2i-node
docker build -t base-nodejs .
s2i build git@github.com:manojbadam/nodejs-welcome.git base-nodejs hello-nodejs
curl htpp://localhost:8000/healthz
```

### Next Steps
```
1. Try to convert this as a BBC (blessed base container) Image
> Installing all best practises and good libraries in the Dockerfile
> Extending the assembly file to handle more generic scenarios
```

```
2. Try to create a new Java based template Image
> Using the save-artifacts option to store the jar file
```
