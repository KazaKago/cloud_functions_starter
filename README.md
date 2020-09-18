# cloud_functions_starter
"Cloud Functions" Starter Kit.

## Run Locally

```sh
$ ./gradlew runFunction -PrunFunction.target=com.kazakago.cloud_functions_starter.Application
$ curl http://localhost:8080/
```

## Deploy Cloud Functions

1. Install gcloud CLI.
    - `$ brew cask install google-cloud-sdk`
1. Login account.
    - `$ gcloud auth login`

```sh
$ gcloud functions deploy cloud_functions_starter --project=kazakago-playground --entry-point=com.kazakago.cloud_functions_starter.Application --runtime=java11 --trigger-http --allow-unauthenticated
```
