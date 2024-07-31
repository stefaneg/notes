# Controlant starting notes

Created: July 22, 2024 7:41 AM
Last Edited Time: July 22, 2024 8:11 AM
Created By: Guðlaugur Egilsson
Last Edited By: Guðlaugur Egilsson

## What is the product?

What exactly is in scope? What does the team say no to, and why?

How to figure this out:

- Extract anything that exists
- One-one with all teams (leads)
- Document 2-3 suggestions
- Workshop

## Choice Architecture.

The aim of a platform team is to make their platform attractive, by making it cheaper and easier to get CI/CD, running platform and observability than by building your own platform. Should not be the only choice though. Building your own for a new service/deliverable should be an explicit sell.

Standardized logging, monitoring and metrics support is something that needs to be looked into very explicitly.

QA: Work with Ben Gruber to figure out how to gauge the quality of QA of different teams.

## Unsolved problems

### Disaster recovery
Disaster recovery exercises in teams.
Definitely create a plan for Gitlab and Grafana.

### Depreciation of old accounts.
Need to list capabilities and responsibilities still there and form a plan around them.
Explore state of "deprecation know-how and culture" and figure out ways to help improve.

### Responsibilities
Technical Leadership:

- Foster a collaborative and supportive environment where team members can grow and
excel.
- Empower team members by providing clear technical direction, guidance, and resources to
achieve project goals.
- Architect and design the product with support of the team and architects.
- Guide & Coach agile teams on continuous integration and automated deployment.
- Design, develop, and maintain the developer tools and platforms that improve productivity
and efficiency.
- Create and maintain CI/CD pipelines to automate build, test, and deployment processes.
- **Implement observability tools and frameworks for monitoring, logging, and alerting to
ensure system health and visibility.**
- Develop and maintain internal tools and services to streamline development workflows.
- Evange Implement observability tools and frameworks for monitoring, logging, and alerting
to ensure system health and visibility.
- Evangelize best practices in code quality, testing, and deployment across the organization.
- Stay up to date with emerging technologies and industry best practices related to developer
platforms, Kubernetes, AWS services, and serverless computing.
- Write automated tests, set up, maintain, and operate test automation software and
frameworks on multiple application platforms.

### Product leadership:

- Define and communicate the product vision, strategy, and roadmap for the developer
platform.
- Prioritize features and enhancements based on business goals, user needs, and technical
feasibility.
- Gather requirements and feedback from development teams to ensure the platform meets
their needs and expectations.
- Create and manage the product roadmap, detailing upcoming features and enhancements.
- Collaborate with cross-functional teams to ensure successful delivery of features.
- Monitor product performance and user satisfaction, making adjustments where needed.
- Communicate product updates, progress, and roadmaps to stakeholders.
- Develop and maintain comprehensive documentation for developer tools, CI/CD processes,
and automation frameworks.