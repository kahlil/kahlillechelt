
---
date: 2019-07-08T14:29:08.011Z
title: "Build a Slack slash command app with Zeit’s Now"
---

First of all: [**Now**](https://zeit.co/now) is so flipping great it’s not even funny. Basically it is this: 

You write your app, type `now` and it's deployed. You get back the URL under which it is deployed and that’s that. Every other deployment results in a new deployment under a new URL.

The latest deployment is always aliased to a URL that doesn’t change and that’s the address to your app or API.

If you hook up Github, your branches get deployed automatically as immutable deployments. The alias of those deployments contains the branch name. Every push results in a new deployment.

Now is a perfect fit if you want to create a slash command app for Slack.

---

Slash commands are super simple. When you send off a message like `/mycommand yey` all the command does is sending a post request over to a URL with your command and then prints out the response to you in Slack.

I used [**Micro**](https://github.com/zeit/micro) (also made by our buddies at Zeit) to set up the API. Micro is a small no-config Node tool that allows you to create a microservice in no time. All you need to do is to write the function that takes the request and start the microservice with the `micro` command and you're good to go. 

Now comes with [initialization templates](https://zeit.co/blog/now-init) that have configurations for different tools, frameworks, static site generators, etc. One of them is called `node-micro` which configures Micro for Now. In order to use it, all you have to do is type `now init` and then choose `node-micro`.

It works out of the box. If you start the `now dev` and curl `localhost:3000` you get the hello world message as a response.

You can deploy that by just typing `now` on the terminal or by hooking up now with your GitHub repository.

---

Next, all you have to do is to configure your [**Slack slash command**](https://api.slack.com/slash-commands). Give it a name and a slash command and the endpoint URL. In our case it would be the alias that was generated. The alias always points to the latest deployment. 

When you use that slash command it will post back that hello world message back into your Slack chat as a response. 

Now you are ready to take over the world with your Slack slash command!

