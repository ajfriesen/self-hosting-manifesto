
# Pragmatic Self-Hosting Manifesto

This is a manifesto for the pragmatic self-hoster.
It is a collection of rules which should be followed to make your life easier.
Be aware that these rules are not absolute.
They are just a guideline to make your life easier.

## Keep it simple

Understand what you are doing.
Do not blindly follow tutorials.
You have to understand what you are doing.
This will make your life easier when things break.

That level of simplicity might change over time depending on your knowledge you will gain over time.

## Design your system for time off and leisure time 

Technology should be a tool to make your life easier.
Do not be a slave to your technology.

Build systems which can be left alone for at least a few weeks.
There are times in live where you actually do not want to tinker with tech.
Be it enjoying outside activities, family duties, school, etc.
That is okay.

## Do not use too many machines

You do not need a rack with multiple servers.
You will be amazed how much you can do with a single machine with 4 cores.
And since technology is evolving you will be able to do more and more with a single machine since core count is just going up.

## You do not need clusters

We are in a time where everything is clusters.
Clusters solve problems with the downside of complexity.
You are not an enterprise where large teams take care of these clusters.

## You do not need Kubernetes at home

Kubernetes is a great tool.
However, it is a complex tool.
You do not need it at home.
Use docker-compose or similar tools to manage your containers.

## Have dedicated hardware for certain tasks

Sometimes it is easier to have dedicated hardware for certain tasks to make things less complex.
Virtualized firewalls for example make it more complex to update your hypervisor.

## Automate, but do not automate everything

Automation is our friend.
However, automation heavily benefits from the pareto principle.

- 20% of the effort/time will give you 80% of the benefits.
- The remaining 20% automation will cost you 80% of the effort/time.

In hardware and infrastructure we often have the chicken egg problem.
This makes 100% automation inherently really hard and therefore time consuming for the last few percent.

You are not a business, where this might be needed.
Value your time.

## Do not judge tools based on their programming language

It does not make sense to not use software just because it is written in a programming language you happen to not like.
Use it if it solves your problem.

## Databases are not bad

There are some people out there who think databases are bad.
Therefore all software using databases is bad.
Databases have reason to exists. Period.

You still may choose to use plaintext solution for whatever you would like to achieve.
However, that does not make databases a bad technology.

## Backups

Have them.
Seriously.

It does not have to be the perfect 3,2,1 rule.
Just think about what has value to you and what you are okay to loose or setup again.

## Basic security

- Do not use SSH logins with password.
- Do not open ports if not needed.
- Use a firewall.
- Use a VPN.

## Update your systems/software

You need to update your systems regularly.
This is especially true for public facing systems.
This one of the task which should be automated.

## High uptime is a bad metric

Do not brag about a high uptime.
If you do not reboot regularly you do not know if your system is reboot safe and come up after a reboot.

Most kernel updates require a reboot.
If you do not reboot your might be running an outdated kernel and be open to vulnerabilities.
(There are exceptions with live patching.)

## Do not judge others for their setup

You are always missing context when someone is explaining their particular setup.
Be it context in time, knowledge or other circumstances at that time.
Most decisions in life were not made deliberately stupid.
It just happened to be that the decision now would not be the best to begin with.

## Do not listen to these rules when the goal is learning

When you want to learn a new technology you do not have to listen to these rules.
Gaining experience by running a complex cluster at home is a valid reason.

It is not a question of if it will break, but when it will break.
Just be aware of that.
