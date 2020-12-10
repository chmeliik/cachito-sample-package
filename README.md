# cachito-sample-package

Test how cachito handles symlinks

```shell
curl http://localhost:8080/api/v1/requests \
    -X POST \
    -H 'content-type: application/json' \
    -d '{
          "repo": "https://github.com/chmeliik/cachito-sample-package/",
          "ref": "38eebbc1be3b12eff8c4a73aca4a279ad229a9e5",
          "pkg_managers": ["pip"],
          "packages": {
            "pip": [
              {"path": "src"}
            ]
          }
        }'
```
