---
layout: post
title: clone from multiple github accounts with ssh
date:   2018-09-30 17:04:00 +0200
categories: git github
---

You have multiple github account and want to push and pull without having to type your password all the time?

If you use ssh this is actually possible with a little workaround:

Create a config with within your ssh folder `~/.ssh/config` with the following contents:
 
{% highlight bash %}
Host github.com
	HostName github.com
	User git
	IdentityFile ~/.ssh/private_github

Host github.com-work
	HostName github.com
	User git
	IdentityFile ~/.ssh/work_github
{% endhighlight %}

You can set the appropriate hostname like this: `git remote set-url origin git@github.com-work:company/awesome_project.git`

To see your remote url, you can use `git remote -v`.

From now on every pull from the `github.com-work` host will use the `work_github` ssh key.
