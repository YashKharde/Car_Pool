# carPooling

FareShare is a learning project for finding travel companions, coordinating shared cab seats and explaining fare splits.

Public GitHub repository: [YashKharde/Car_Pool](https://github.com/YashKharde/Car_Pool). The local project folder remains `carPooling`.

**Current step:** S01 product rules documented. Application implementation starts in S02.

## Start here

- [Product scope](docs/product.md)
- [Business rules](docs/business-rules.md)
- [Example user journeys](docs/user-journeys.md)
- [Progress and next step](docs/progress.md)
- [How we work and commit](CONTRIBUTING.md)
- [Architecture scope decision](docs/decisions/001-scope.md)
- [Step S01 record](docs/steps/S01.md)

## Repository layout

```text
backend/          Spring Boot application, later extracted services
frontend/         Angular application
infrastructure/   Docker, NGINX and AWS infrastructure
contracts/        API and event contracts
docs/             Decisions, step records, roadmap and guides
```

S01 creates documentation and directory boundaries only. There is no runnable application yet; no backend/frontend tests or cloud deployment have occurred.

## Target stack

Java, Spring Boot, Angular, MySQL, Kafka, Redis, Docker, NGINX and AWS. Supported compatible versions will be selected and recorded during setup, rather than guessed in advance.

We start with one application organized by feature, complete a ride journey, then extract three focused services. MySQL is authoritative for reservations. Kafka handles background events; Redis supports sessions, caches and rate limits.

## Current limits

One city, named meeting points, organizer approval, one seat per rider and equal fare splitting. The group arranges its own cab. The app does not process payments, verify transfers, track live GPS or guarantee personal safety.

Security is implemented and tested throughout. No vulnerability-free guarantee is claimed.
