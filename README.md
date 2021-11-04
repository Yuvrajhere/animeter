# Habbit Web App
[Website](https://habbit.co.in) - [Jenkins](https://jenkins.habbit.live) - [Spinnaker](https://spinnaker.habbit.live)

[![codecov-coverage](https://codecov.io/gh/habbit-tech/habbit-webapp/branch/main/graph/badge.svg?token=TR0QG39ADU)](https://codecov.io/gh/habbit-tech/habbit-webapp)
![CI Tests](https://github.com/habbit-tech/habbit-webapp/actions/workflows/tests.yaml/badge.svg)

This repository contains the source code for the Habbit Web Application.

## Build & Deployment


--> Devs 

--> Push to `main` branch 
  
--> [Jenkins Build](https://jenkins.habbit.live) (same creds as Django Dashboard) 
  
--> Push Image to AWS ECR 
  
--> [Spinnaker Deployment Pipeline](https://spinnaker.habbit.live) (login via github)
  
      - Test and verify change in staging env
      - Approve/Reject deployment to prod
      
--> `If` approved `then` changes pushed to PROD `else` deployment terminates 


## Setup

```
git clone https://github.com/habbit-tech/habbit-webapp
cd habbit-webapp
yarn
```

## Development Server

```
yarn dev
```

## Storybook

```
yarn storybook
```

## Test

```
yarn test
```

### Coverage

```
yarn test:coverage
```

## Lint

```
yarn lint
```

## References

-   [Nextjs](https://nextjs.org/docs/getting-started)
-   [SWR](https://swr.vercel.app/)
-   [Doc Comments](https://tsdoc.org/)
-   [Storybook](https://storybook.js.org/docs/react/get-started/introduction)
-   [React Style Guide](https://www.thenewboston.com/style-guide/react) & [SCSS Style Guide](https://www.thenewboston.com/style-guide/css)
-   [Linting Setup](https://robertcooper.me/post/using-eslint-and-prettier-in-a-typescript-project)
