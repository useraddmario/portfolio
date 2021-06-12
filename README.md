![portfolio diagram](https://raw.githubusercontent.com/useraddmario/portfolio/main/Portfolio_Site.jpg)


# Simple Hugo Site

Just a simple website project with links to my professional social media.  The site is created from source markdown files using Hugo, a static site generator.  I built this as part of a plan to use this workflow to run some kind of automated documentation of projects in the future.  I should be able to just generate markdown in each CI step and spit out a documentation wiki at the end.

## Automation

I use CircleCI to orchestrate the build/update sequences for the Hugo website output and AWS infrastructure as well as cleanup of the old version.

## Infrastructure

Everything AWS is built/updated with two Cloudformation stacks, minus ACM which was already configured.  

#### AWS Services used include
* S3
* Route53
* CloudFront
* ACM

### Lacking

I still need to add testing steps, monitoring, and alerting; after my other projects are polished, I guess.


### Built With

- [Circle CI](www.circleci.com) - Cloud-based CI/CD service
- [Hugo](https://gohugo.io/) - Open-source static site generator; markdown to HTML
- [Amazon AWS](https://aws.amazon.com/) - Cloud services
- [AWS CLI](https://aws.amazon.com/cli/) - Command-line tool for AWS
- [CloudFormation](https://aws.amazon.com/cloudformation/) - Infrastrcuture as code
