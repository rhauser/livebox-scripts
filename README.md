# Scripts using the Orange Livebox REST API

Run the scripts either by using `pipenv shell` in this
directory, or `pipenv --bare run ../livebox-scripts/add-pinhole ...`.

## One time preparation

```shell
sysbus -config
```

It will store the parameters to access the API in ~/.sysbusrc.

## add-pinhole - Add an IPv6 firewall entry

