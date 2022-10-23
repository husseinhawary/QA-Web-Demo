

## Getting Started

### Prerequisites

The following software are required:

- nodejs.
- vs code.
- docker.

### Installation

1. Clone the repo using below URL

```sh
https://github.com/husseinhawary/QA-Deliveroo-Demo.git
```

2. Navigate to folder and install npm packages using:

```sh
npm install
```

## Running local and show the report

1. Run local
```JS
npx playwright test
```
2. Run local in non headless mode
```JS
npx playwright test --headed
```
3. Show the report
```JS
npx playwright show-report
```

## Docker
  The project integrated with github actions and you can see the runs build and rerun it from here 
```JS
https://github.com/husseinhawary/QA-Deliveroo-Demo/actions
```

## Docker
  I added the Dockerfile but I didn't complete testing it locally because it takes a lot of time so I am not turst if it works or there is any issues in integration
  - These steps which I proceed in it to run the test dockerized but didn't complete it.
```JS
docker build -t playwright-docker .
```
```JS
docker image ls
```
```JS
docker run -it playwright-docker:latest npm run test
```