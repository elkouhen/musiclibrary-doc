# Configuration 

## Compte AWS

### Configurer les credentials AWS

``` ini
# Extrait fichier ~/.aws/credentials
[profile_cours_serverless]
aws_access_key_id = XXX
aws_secret_access_key = XXX
region = eu-west-3
```

### Choisir le profile AWS

Sous Linux

``` bash
export AWS_DEFAULT_REGION=eu-west-3
export AWS_DEFAULT_PROFILE=profile_cours_serverless
```

Sous Windows

``` bash
set AWS_DEFAULT_REGION=eu-west-3
set AWS_DEFAULT_PROFILE=profile_cours_serverless
```

### Vérifier la config AWS

``` bash
aws sts get-caller-identity
{
    "UserId": "629923658207",
    "Account": "629923658207",
    "Arn": "arn:aws:iam::629923658207:root"
}
``` 
