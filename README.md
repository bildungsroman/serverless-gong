# The Serverless Gong! 🔔

A serverless gong with GitHub and Slack webhooks - made for the [No Server November Challenge](https://serverless.com/blog/no-server-november-challenge/).

## Links

* Read the [Serverless Webhooks Tutorial](https://docs.stackery.io/docs/tutorials/serverless-webhooks/) to get started
* Read the [blog post on the serverless gong](https://www.stackery.io/blog/serverless-gong/) for more on this project

## Deploy this to your AWS account

You can deploy this application to your own AWS account using the following two Stackery CLI commands:

`stackery create` will initialize a new repo in your GitHub account, initializing it with the contents of the referenced template repository.

```
stackery create --stack-name 'serverless-gong' \
--git-provider 'github' \
--template-git-url 'https://github.com/stackery/serverless-gong' 
```

`stackery deploy` will deploy the newly created stack into your AWS account.

```
stackery deploy --stack-name 'serverless-gong' \
--env-name 'development' \
--git-ref 'master'
```
