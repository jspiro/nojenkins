# No Jenkins

No Jenkins is the best way to avoid using Jenkins and Groovy to do arbitrary
things on a schedule.

No Jenkins leverages and extends the
[nocode](https://github.com/kelseyhightower/nocode) framework.

## Getting Started

Whenever you think "I could do this with Jenkins," reconsider and use
No Jenkins instead.

Begin by copying the shell script you already made from your POC
into No Jenkins. Run it through `shellcheck`, and then call it from the Crontab.

You're done, and you did it without Jenkins!

## Deploying

You know how people always say "well it works from my machine," usually in
contrast with difficulties trying to deploy "it" to Kubernetes or EC2?

You may be surprised to learn that No Jenkins runs _great_ from your machine,
especially in a production environment.

There are two supported configurations:

### In the cloud (preferred)

1. Literally ship your machine to a colo and make it someone else's problem.

Be sure to save some of your budget for Remote Hands.


### On-prem

1. Install `ngrok` and manually configure your DNS to point to it.
2. Move your machine to the Harry Potter room under your stairs.

You'll want to pay for `ngrok` if you're lazy so the endpoint doesn't change.

Otherwise, use No Jenkins to periodically restart `ngrok` and update the DNS.
Be sure your DNS provider credentials are embedded directly in the shell script,
since cron jobs start with nearly empty environments.

## Contributing

Nah, I think we're good.
