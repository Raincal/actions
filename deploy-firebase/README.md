# Deploy Firebase

This action deploys a static site to Firebase Hosting.

## Secrets

- `FIREBASE_TOKEN` - *Required* Generate a Firebase CLI token using `firebase login:ci`

## Usage

```workflow
workflow "Deploy blog" {
  on = "push"
  resolves = ["Deploy to Firebase"]
}

action "Build blog" {
  uses = "./.github/build"
}

action "Deploy to Firebase" {
  uses = "Raincal/actions/deploy-firebase@master"
  needs = ["Build blog"]
  secrets = ["FIREBASE_TOKEN"]
}
```
