---
layout: post
title: Set Emacs with Purcell's Configuration
---

<div class="message">
     The BEST WAY to study Emacs is to imitate a genius,while others think it should be learning step by step naturally.
</div>

## Prerequisites

Ensure you have installed Subversion and Git,and made up your mind to be a NewBee Emacser/Developer.

## Fork the repository from Github

View the github repository from :https://github.com/purcell/emacs.d,

then fork it to your own github repository.You should manage the Emacs plug-ins with github.

## Clone the repository to localhost

{% highlight sh%}

## Move your own repository to somewhere else,preventing conflicts to new configuration
mv .emacs.d .emacs backup/

## Clone repository
git clone https://github.com/githubaccount/emacs.d.git ~/.emacs.d

## Change to the .emacs.d directory
cd .emacs.d

##Initialize with Github
git submodule update --init
{% endhighlight %}

## Initialize the plug-ins automatically

Open Emacs with your own account and wait for the automatic initialization completed!

## Merge your own configuration with it

After the configuration,there's are several distributed configuration files in ~/.emacs.d/lisp,and reference them by ~/.emacs.d/init.el.

This means you shouldn't custom your Emacs with .emacs anymore but init.el and other .el files in ~/.emacs.d/lisp.Also,the resource packages need to be put in that directory too.

Ehhh,maybe Purcell have set a ordeal for followers. The default color theme tastes really bad,as it's a bombing to my eyes.You can either change the init-themes.el or add your own themes.

You can append shortcuts in init.el or make a dedicated file.

## Have fun!
