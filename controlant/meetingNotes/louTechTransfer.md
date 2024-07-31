# Knowledge transfer with Lou

Created: July 19, 2024 1:49 PM
Last Edited Time: July 30, 2024 10:23 AM
Created By: Guðlaugur Egilsson

Main tools ? Main skills that you would say are required ?

K8S. Deployment of code exclusively through terraform. Serverless framework JS. 95% terraform. 5% gitlab CI. Gitlab. Vault. AWS secret manager is legacy. Vault for temp credentials. Static secrets. A few users left with static secret. No users with admin access. Teams have only deployment access to UAT and live.

Pentests. Does not know who.

Gitlab - public, internal, private.

What is the scope? What do you do? What do you say no to?

Hacks ?

Private Link - VPC

Gitlab using AWS Private link

Gitlab runners in catapult accounts. Run integration tests.  [https://blog.aqd.is/2023/10/gitlab-privatelink](https://blog.aqd.is/2023/10/gitlab-privatelink)

Open source projects on github.

Hono - ingress team.

Main challenges in the last year or so?

Mostly organisational. Lack of focus and direction. Oli

Multi account - access control.

Sandbox tenant.

Launch darkly. Test automation.

Catapult accounts. Old accounts.

It is a wish to move away from old accounts. AWS Event Bus.

Azure has their own infrastructure group. AD applications.

[controlant.com](http://controlant.com) on aws side. route53. [bi.controlant.com](http://bi.controlant.com) on azure.

Network connectivity to azure. Completely clickops.

Andri Arnason Azure devops. Aquired a company using PowerBI ?

What would you say is most in need of attention ?

**Evangelise the use of deprecation. Study how that can be achieved.**

**Disaster recovery exercises. Absolutely zero.**

Search for Recovery Exercise on confluence site.

Developer platform is stable enough. In need of a vision of where it is going next. What about the old accounts ?

The company does not understand deprecation.

Coralogix.

Terragrunt.

Who are the key stakeholders I should connect with regularly?

Architects. Elvar and Gisli. Open to ideas. Tech leads around the company. 10 ish. A lot of churn. Halldora set up group. Ben Gruber. QA engineering team. SonarQube. Andrew.

Best training material that matches your way of thinking ? Books, inspirations ?

Official documentation. CCP Optimise for maintaining one project. Nicholas.

Redundancy, recovery strategies, chaos monkeying, etc?

Disaster recovery exercises. Absolutely zero.

No disaster recovery plan in place for Gitlab.

Not for databases either.

Please tell me all internal code-names that would be useful to me to know. Perhaps in a follow up post ?

Search for Catapult, Glossary in confluence pages. VSO Vault Secret Operators.

Workspaces vs directories for managing various environments ? Other ?

Are you using HCP ? If not, how are you managing state and state locking? S3 and Dynamo.

Can you show me the basics of how you are using Vault ? What is the authorisation model ? Secret management ?

Credential management ?

1Password.

We run Grafana and Gitlab. Driven by AD.

AWS SSO not connected to AD.

Might want to evaluate connecting to AD.

Check if Lou is still there in terraform.

Meaning our personal access keys, temporary log ins etc.

Compliance and regulation. Auditing?

AWS cost management and optimization strategies in place?

Automated QA methods in place ? For example automated created/destroy of stack(s).

Ingress / Egress definitions, conventions, monitoring, logging, etc.

How is IaS code promotion performed ?

Why no variables ?

Why Rust ?

Terraform upgrade strategy ?

Enumerate 3rd party tools in use.

Naming conventions ?