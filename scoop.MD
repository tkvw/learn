# Scoop.sh 

Install software in Windows without poluting the system (user based). 
Software is installed using a descriptor json file. A bundle of these descriptors form a bucket and 
are stored in git. Main is the standard butcket and is available by default. 

## Install

Invoke-Expression (New-Object System.Net.WebClient).DownloadString('https://get.scoop.sh')

## Buckets

```
scoop bucket add extras 
scoop bucket add jetbrains
```

## Install 

```
scoop install curl 
scoop install git
scoop install vscode
scoop install jq
```

## Install c# environment

```
scoop install azure-cli
scoop install azure-functions-core-tools
scoop install dotnet-sdk
```
