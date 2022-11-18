# Azure AKS User Management WebApp Demo

## Build app

```bash
# to build 
./mvnw package

# create image
cd ..

docker build --pull --rm -f "azure-aks-usermgmt-webapp-demo/Dockerfile" -t usermgmt:0.1.1 "azure-aks-usermgmt-webapp-demo"

docker tag usermgmt:0.1.1  jkolonkova/azure-aks-usermgmt-webapp-demo:1.0

docker push jkolonkova/azure-aks-usermgmt-webapp-demo:1.0

```

### Prerequisites

On windows:

- make sure wsl2 is used & preffered distribution is installed
- Activate this distribution in docker desktop
- install java & make sure JAVA_HOME env is set

```bash
sudo apt install default-jdk
sudo apt install default-jre
```
