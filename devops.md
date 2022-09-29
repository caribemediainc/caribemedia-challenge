# DevOps Challenge

The assignment is designed to check your coding, problem-solving and cloud design skills . We suggest you spend a maximum of 10-14 hours on it.

Things we require your work to have:

- Using of IaaS (Infraestructure as a Code)
- Code organization (modularity, dependencies between modules, etc)
- Good practices on Continuous Integration/Deployment process
- Exception handling and logging
- Good and readable documentation

## Introduction

Caribe Media needs a software that allows the management of the internal tasks as well as the sales management. For this purpose, the company has chosen to use an Open Source solution: **Odoo**.

### Odoo

Odoo is a suite of open source business apps that cover all your company needs: CRM, eCommerce, accounting, inventory, point of sale, project management, etc. Odoo's unique value proposition is to be at the same time very easy to use and fully integrated.

## Requirements

Your job as DevOps Craftman is to deploy this solution to the cloud infrastructure through Docker containers and Kubernetes that guarantee the scalability and high availability of the system. Every server log must be monitored through a portal or terminal cli. The database must be protected against any security attack.

### Tasks

1. Expose a Dockerized Odoo instance to a public and accesible IP on the cloud. Feel free to use any additional tools to get the job done.

## Deliverables

1. Use GitHub Actions.
2. Use the cloud provider of your preference to deploy (preferably GCP). Make sure we can play with public IP the Odoo Portal.

## Nice to have (not required)

1. Decouple Database from Odoo server, use a Potsgres as a Service instead.
2. Use some tool to monitor your infraestructure and logs.

## References

- [What is Odoo?](https://www.odoo.com/)
- [Docker and Odoo](https://hub.docker.com/_/odoo)
- [Odoo Runbot](https://runbot.odoo.com/)
- [Why deploy Odoo as a Docker container](https://www.brainvire.com/blog/deploy-odoo-as-a-docker-container/)
