# Components_NiFi-registry

Initial deploy of nifi-registry. A default container from the docker hub is deployed as a single instance.
Currently the nifi-registry from the components_nifi repo is used

## Manually deployment command:
```ps1
kubectl apply --namespace=odala-staging -f ./deployment-nifi-registry.yml
```

## CICD (GitLab)
The release process is automated if you use the cicd pipepeline: .gitlab-ci.yml, the pipeline is triggered when changes are pushed to a branch with prefix odala-staging / odala-production

Secrects are set during deployment (GitLab cicd) and taken from GitLab group settings CICD variables.

## License
for the ODALA project.

© 2023 Sirus

License EUPL 1.2

![](https://ec.europa.eu/inea/sites/default/files/ceflogos/en_horizontal_cef_logo_2.png)