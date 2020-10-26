# Sloop: the journey from hackathon idea to Open Source project
Speaker: Min Wang, Lead Software Engineer, Salesforce

Monitoring and retrieving history data in Kubernetes is challenging, when a resource is terminated its corresponding logs will disappear. Existing tools either lack functionality or they are expensive making them unaffordable in the current economic environment. How can we develop a free tool that helps users get Kubernetes history data? This is the inspiration for our open source project: Sloop.

### Notes

- Using Kubernetes to handle customer application deployment 
- Problems
    - Don’t have visibility into what pod is deleted
    - What pod is hosting the application
    - Logs not available once pod is deleted
- Sloop - started as a hackathon idea
    - Wrote simple CLI tool to use local disk as database and store some pod info in the database
    - Once pod is deleted, you can access that info from local disk like pod history
    - Kube API -> Ingress constantly calls API -> data process like resource summary -> BadgerDB -> Disk
- UI
    - Different colors to indicate health of resources
    - Links to access logs - help in debugging
- Project available as open source tool
    - Check license of dependencies used - LicenseFinder
    - CI tool - Travis CI - runs job to check your PR 
    - DockerHub - Public Image - helpful for docker image
    - Gorelease - Release
    - All tools are free
- Things learned
    - Embrace open source
    - Design for majority - use open sourced tools
    - Make services configurable - integrate with tools / plugins
    - Get feedback from internal resources - UX team review, legal review, demo to audience
    - Maintain repo and look for feedback - open issue, customer feedback
    - Make it visible - meetups, talks, demos, social media
