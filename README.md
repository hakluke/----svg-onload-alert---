Welcome to the AWS CodeStar sample static HTML website
==================================================

This sample code helps get you started with a simple static HTML website
deployed by AWS CodeDeploy and AWS CloudFormation to an Amazon EC2 instance.

What's Here
-----------

This sample includes:

* README.md - this file
* appspec.yml - this file is used by AWS CodeDeploy when deploying the website
  to EC2
* scripts/ - this directory contains scripts used by AWS CodeDeploy when
  installing and deploying your website on the Amazon EC2 instance
* webpage/ - this directory contains static web assets used by your website
  * index.html - this file contains the sample website
* template.yml - this file contains the description of AWS resources used by AWS
  CloudFormation to deploy your infrastructure
* template-configuration.json - this file contains the project ARN with placeholders used for tagging resources with the project ID

Getting Started
---------------

These directions assume you want to develop on your local computer, and not
from the Amazon EC2 instance itself.

To work on the sample code, you'll need to clone your project's repository to your
local computer. If you haven't, do that first. You can find instructions in the
AWS CodeStar user guide.

1. Open `index.html` from your cloned repository in a web browser to view your website.
   You can also view your website on the AWS CodeStar project dashboard under Application
   endpoints.

What Do I Do Next?
------------------

You can start making changes to the sample static HTML website. We suggest making a
small change to /webpage/index.html first, so you can see how changes pushed to your
project's repository are automatically picked up by your project pipeline and deployed
to the Amazon EC2 instance. (You can watch the progress on your project dashboard.)
Once you've seen how that works, start developing your own code, and have fun!

Learn more about AWS CodeStar by reading the user guide.  Ask questions or make
suggestions on our forum.

User Guide: https://docs.aws.amazon.com/codestar/latest/userguide/welcome.html

Forum: https://forums.aws.amazon.com/forum.jspa?forumID=248

How Do I Add Template Resources to My Project?
------------------

To add AWS resources to your project, you'll need to edit the `template.yml`
file in your project's repository. You may also need to modify permissions for
your project's worker roles. After you push the template change, AWS CodeStar
and AWS CloudFormation provision the resources for you.

See the AWS CodeStar user guide for instructions to modify your template:
https://docs.aws.amazon.com/codestar/latest/userguide/how-to-change-project.html#customize-project-template

What Should I Do Before Running My Project in Production?
------------------

AWS recommends you review the security best practices recommended by the framework
author of your selected sample application before running it in production. You
should also regularly review and apply any available patches or associated security
advisories for dependencies used within your application.

Best Practices: https://docs.aws.amazon.com/codestar/latest/userguide/best-practices.html?icmpid=docs_acs_rm_sec
