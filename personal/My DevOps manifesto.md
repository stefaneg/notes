# My DevOps manifesto

“You write it, you operate it”.

Best fit for troubleshooting, knows the inside best.

Written software - your deployments.

Specific purpose software - third party software, special purpose for the team.  Such as queues, monitoring (ELK stack, Sentry, Grafana, etc), Kubernetes, etc. 

General purpose software - operating systems, VM clusters.

Blue areas “developers”, Mixed areas “platform team”, Green areas “ops team”.

DevOps is the bridge between the instability of Development and the stability of ops. One lane of that  bridge is built with  CI/CD pipelines. It starts in version control, the deck is a CI automation tool, the pillars are automated quality checks, most often classified into static analysis and automated testing, and the other end is automated deployments into production systems.

The other lane on the bridge is built with monitoring, metrics and usage analysis tools. Together, these enable DevOps oriented teams to create rapid feedback loops which function to accelerate response times to production issues.

Perhaps more importantly, feedback loops like this facilitate accelerated learning of developers, who are already experts in both the technology and the domain problems they are solving. This enables deeper learning of the capabilities and limitations of the technology they are using, as well as enabling deeper learning intricacies of the domain problem, including the actual usage patterns and insights into user expectations and needs.

Platforms are what developers create to make the crossing of this bridge smoother, or to improve the developer experience around all the responsibilities around, delivering, operating and monitoring written software.

In order to leverage this learning, members of DevOps teams must have agency to apply that learning. The challenge then comes down to one of governance models. Software development teams are often working with feature roadmaps, with schedules attached. Sometimes termed “feature factories”, this model is challenging to work with in a DevOps team, as the pressure of delivering features on schedule usually pushes aside the attention and time required to attend to monitoring of systems, and to absorb the learning that is to be gained there.

This is where the “product operating model” of Marty Cagan comes in strong. By giving teams agency to focus on business problems rather than feature delivery, I believe that the pressure naturally shifts to that of learning and acquiring the knowledge required to solve those problems. Hence leveraging the power of DevOps to enable to solve problems faster, stabilize new features faster, and acquire knowledge faster and more reliably. Which can be used to solve tomorrow’s business problems.