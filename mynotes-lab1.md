# LAB1

## upload blueprint (mix of code and template)

``` bash
cfy blueprints upload -b hello hello.yaml
```

``` bash
helm install --name hello hello_chart
```

## list blueprints

``` bash
cfy blueprint list
```

``` bash
helm list
```

## add label

``` bash
cfy blueprints labels add training:lab1 hello
cfy blueprint list
```

``` bash
helm
```

## create a deployment

``` bash
cfy deployment create hello -b hello
cfy blueprint list
```

``` bash
helm
```

## execute

``` bash
cfy exec start install -d hello
```

``` bash
helm
```

## check the output

``` bash
cfy deployments output hello
```

``` bash
helm
```

## deployment update

``` bash
cfy deployments input hello
cfy deploments update -i 'webserver_port=8800' hello
```

``` bash
helm
```

## stop the execution

``` bash
cfy executions start uninstall -d hello
```

``` bash
helm
```

## delete the deployment

``` bash
cfy deployments delete hello
```

``` bash
helm
```