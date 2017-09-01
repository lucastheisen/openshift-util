# An OpenShift client inside of a Docker container

## Building
```powershell
# Run from this folder
docker build . --tag openshift-client
```

## Running
```powershell
docker run -it --rm `
    -v /var/run/docker.sock:/var/run/docker.sock `
    openshift-client
```