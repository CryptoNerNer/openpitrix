# openpitrix

OpenPitrix addresses the problem of packaging, deploying, and managing applications across different cloud and runtime environments. It provides a common workflow for application versions, marketplace publishing, and deployment from one platform.

> **Status:** This standalone project is based on `openpitrix/openpitrix`. The donor project is deprecated, and its features were merged into [KubeSphere](https://kubesphere.io/).

## Features

- Package Kubernetes, microservice, and serverless applications.
- Deploy application versions to runtimes such as AWS, Azure, Kubernetes, QingCloud, OpenStack, and VMware.
- Publish application versions through an application marketplace.
- Manage application versioning across creation, testing, publishing, and deployment stages.
- Assign organization roles for administrators, developers, ISVs, and regular users.

## Installation

Install Go and Git, then clone the repository and build its packages:

```bash
git clone https://github.com/openpitrix/openpitrix.git
cd openpitrix
go mod download
go build ./...
```

The project also depends on the deployment environment and runtime integrations you plan to use. Consult the repository configuration and deployment documentation before running it in a shared environment.

## Usage

Build or run the OpenPitrix command from the repository root. Use `--help` to inspect the options available in the checked-out version:

```bash
go run . --help
go run . --config ./config.yaml
```

A configuration file can define the services and runtime settings required by your deployment. Use the application workflow to create a version, test it, publish it to the marketplace, and deploy it to a supported runtime.

## License

openpitrix is licensed under the Apache License 2.0. This project is based on [openpitrix/openpitrix](https://github.com/openpitrix/openpitrix), which was released under the Apache-2.0 license. See [LICENSE](LICENSE) for the full license text and attribution details.
