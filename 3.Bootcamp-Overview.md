# WemaDevOps - DevOps Bootcamp Overview

### Overview of the DevOps processes

- `DVCS` - Git / GitHub / GitLab / Bitbucket / Azure repo / Code commit
- `Git basic` / Git branching strategies - Feature branching strategy, Trunk-based development, GitHub Flow, Git Flow

`Pipelines` - Git Actions / Jenkins / GitLab CI / Code Pipeline / Azure DevOps / CircleCI

- `Testing` - Unit testing / Junit-maven, selenium, `checkov`, `tfsec`, `trivy`, SonarQube, pytest
- `SAST Vs DAST` - Shift Left
- `Deployments` - ArgoCD, Ansible, Jenkins / applications / modules - k8s, tomcat, docker, containers, docker hub, JFrog, ECR- `integration` / `authentication` / `workflow`
- `Monitoring` - Datadog / Prometheus / Grafana / Jaeger / New Relic/ CloudWatch / ELK
- `Alerting` - Prometheus alert manager / PagerDuty / Slack / ServiceNow / SNS / Email /SMS
- `Ticketing` - bug tracking / issues / Jira / ServiceNow / Atlassian suites - Jira, confluence,
- `Documentation` - notion , confluence

### Scrum ceremonies

- `Daily stand up` - 15-20min / status update / report sprint work - todo/progress/blocked/review/done - story points / epic - contains multiple issues /`Info` - anything that the team needs to know
- `Sprint planning meetings` - 10 working days / 2 weeks - plan for the work to be done / issues and pointing them /
- `Retrospective meetings` - reflections / close of sprint - what went well / how can we improve/ what didn’t go well / lessons learned - feedback on past sprint - take notes on how things are going
- `Design review meetings` - lucid charts / feedback / ask questions / suggestions / critique / security
- `Postmorteum meetings` - after an event / k8s crashed / pods failed / application was offline / after maintenance - investigate what happened / lessons learned - prevent future similar events from happening
- `One-on-one meetings` - manager / progress / goals / how the manager can help you develop as a engineer / struggles - personal / family → hindering you from doing your work

### Projects

- `Stakeholders` - identify / meet stakeholders / product owners / understand what is the need / specifications - what is the `ask` - better understand the project
- `Set priorities / goals` - overall design / create a process
- `Define deliverables` - vpc, k8s, rt53, rds
- `Project schedule` - details of what needs to be done / due dates = project scope
- `Research and design` - pictorial
- `POC` - Proof of Concept / demo / sandbox - team / stakeholder buy in
- `Documentation` - plan for implementation , user docs, how to
- `Implementation` - sprints / in low env first / granular form - plan for roll back
- `Monitoring / feedback` - how is the project performing / customer feedback / bug fixes / customer support
- `Close project` - lessons learned documentation - company docs

### Sample project

- Cloud - AWS
- IAC - cloud agnostic, repeatable, declarative - terraform / cf
- Highly available - accessibility / no downtime - multi-AZ, ASG, LB, CloudFront (CDN)
- Monitor our application - performance
- Modularized - terraform modules
- Collaborative - GitHub / backend
- Deployed into multiple env - dev, stage, prod - us-east-1, us-west-1, us-west-2 / aws accounts
- Deployed through pipelines - GitHub Actions
- website / s3 bucket / CloudFront / notification - s3-B bucket is updated - trigger lambda - send email/ notification backend s3-A bucket - deleted - sns to send email/

### Design

- Terraform - Backend / remote / s3-A state storage
- DynamoDB table for state locking
- VPC -
- s3-B bucket for website hosting
- Lambda for s3-B
- SNS for s3-A
- CloudFront
- IAM

### Modules

- VPC
- Backend / DynamoDB
- S3-B / Website
- Lambda for s3-B
- CloudFront
