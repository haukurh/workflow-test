# workflow-test

A repository where I can test many different Github Action workflows that I might be working on.

## Not much to see here

As stated this is my testing grounds, but in due time this repository could evolve into a GitHub actions recipe book 
of sorts.

## What 'n why?

Little about each workflow / test

### action-output

Here my main goal was to create GitHub action make it easier to sync, only modified files of a directory over to a 
AWS S3 bucket. Then return all the synced files as output of the step which could then be used to create a CloudFront
invalidation request with only the files from previous step.

I created and tested the following actions:

- [GitHub marketplace: haukurh/aws-s3-sync-action](https://github.com/marketplace/actions/aws-s3-sync-w-output)
- [GitHub marketplace: haukurh/aws-cloudfront-invalidation-action](https://github.com/marketplace/actions/prepare-cloudfront-invalidation-batch)

### lftp-deploy

I needed to deploy code to a server over FTP, I didn't like most of the available actions on marketplace so I created
my on own of course.

I created and tested the following action:

- [GitHub repo: haukurh/lftp-action](https://github.com/haukurh/lftp-action)
