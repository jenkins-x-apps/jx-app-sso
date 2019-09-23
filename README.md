# jx-app-sso

This App is for installing SSO for Jenkins X

## Installing 

The Jenkins App can be installed by running:

`jx add app jx-app-sso`

It will ask you to specify a domain, whether you want to use GitHib or Google, a Client ID and for a client secret.

Note that if you choose GitHub you may want to limit dex to specific org, which can be done by editing the created 
`values.yaml` and specifying the orgs like:

```helmyaml
  dex
    connectors:
      github:
        config:
          orgs:
          - jenkins-x
```


