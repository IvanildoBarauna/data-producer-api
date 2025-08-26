## Data Producer API: FastAPI application for sending data to Pub/Sub, used for load testing and triggering pipelines

[![Ask DeepWiki](https://deepwiki.com/badge.svg)](https://deepwiki.com/ivanildobarauna-dev/data-producer-api)

![Project Status](https://img.shields.io/badge/status-done-green?style=for-the-badge&logo=github)
![Python Version](https://img.shields.io/badge/python-3.9-blue?style=for-the-badge&logo=python)
![License](https://img.shields.io/badge/license-MIT-blue?style=for-the-badge&logo=mit)

![Black](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge&logo=python)
![pylint](https://img.shields.io/badge/pylint-10.00-green?style=for-the-badge&logo=python)

[![CI-CD](https://img.shields.io/github/actions/workflow/status/ivdatahub/data-producer-api/CI-CD.yaml?&style=for-the-badge&logo=githubactions&cacheSeconds=60&label=Tests)](https://github.com/ivdatahub/data-producer-api/actions/workflows/CI-CD.yml)
[![IMAGE-DEPLOY](https://img.shields.io/github/actions/workflow/status/ivdatahub/data-producer-api/deploy-image.yml?&style=for-the-badge&logo=github&cacheSeconds=60&label=Registry)](https://github.com/ivdatahub/data-producer-api/actions/workflows/deploy-cloud-run.yaml)
[![GCP-DEPLOY](https://img.shields.io/github/actions/workflow/status/ivdatahub/data-producer-api/deploy-cloud-run.yaml?&style=for-the-badge&logo=google&cacheSeconds=60&label=Deploy)](https://github.com/ivdatahub/data-producer-api/actions/workflows/deploy-cloud-run.yaml)


## Development Stack

[![My Skills](https://skillicons.dev/icons?i=pycharm,python,github,gcp,docker,fastapi,postman&perline=7)](https://skillicons.dev)

## Cloud Stack (GCP)

<img src="docs/icons/cloud-build.png" Alt="Cloud Build" width="50" height="50"><img src="docs/icons/artifact-registry.png" Alt="Artifact Registry" width="50" height="50"><img src="docs/icons/cloud-run.png" Alt="Cloud Run" width="50" height="50"><img src="docs/icons/pubsub.png" Alt="Pub/Sub" width="50" height="50">

- Cloud Build: Continuous Integration and Continuous Deployment (CI/CD) service provided by GCP integrated with GitHub Actions
- Artifact Registry: Private Docker container registry provided by GCP for storing FastAPI image.
- Cloud Run: Fully managed serverless container runtime provided by GCP for running FastAPI Application.
- Pub/Sub: Messaging service provided by GCP for sending and receiving messages between FastAPI and Dataflow pipeline.

## Continuous Integration and Continuous Deployment (CI/CD, DevOps)

![My Skills](https://skillicons.dev/icons?i=githubactions)

## Contributing

See the following docs:

- [Contributing Guide](https://github.com/ivdatahub/data-producer-api/blob/main/CONTRIBUTING.md)
- [Code Of Conduct](https://github.com/ivdatahub/data-producer-api/blob/main/CODE_OF_CONDUCT.md)

## Project Highlights:

- Hexagonal Architecture: Adoption of Hexagonal Architecture to decouple the core logic from external dependencies, ensuring that any current data source can be replaced seamlessly in case of unavailability. This is facilitated by the use of adapters, which act as intermediaries between the core application and the external services.

- Comprehensive Testing: Development of tests to ensure the quality and robustness of the code at various stages of the ETL process

- Fire-Forget Messaging: Use of messaging (Cloud PubSub) in the fire-forget model to manage files generated between the transformation and loading stages, ensuring a continuous and efficient data flow.

- Configuration Management: Use of a configuration module to manage project_id and others env variables, providing flexibility and ease of adjustment.

- Continuous Integration and Continuous Deployment: Use of CI/CD pipelines to automate the build, test and deployment processes, ensuring that the application is always up-to-date and ready for use.

- Code Quality: Use of code quality tools such as linters and formatters to ensure that the codebase is clean, consistent and easy to read.

- Documentation: Creation of detailed documentation to facilitate the understanding and use of the application, including installation instructions, usage examples and troubleshooting guides.

## API Documentation

[Swagger UI](https://ivdatahub.github.io/data-producer-api/)
