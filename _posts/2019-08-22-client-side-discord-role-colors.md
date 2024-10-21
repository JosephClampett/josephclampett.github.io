---
title: 'Client-Side Discord Role Colors'
date: 2019-08-22
permalink: /posts/2019/08/22/client_side_discord_role_colors/
tags:
  - discord
  - customization
  - css
---

This is admittedly a rather lame first blog post, but I thought I would start off with something simple.

Discord servers don't often have the best color schemes, and after a little research and help (completely unfamiliar with CSS) I found there was a very simple and convenient way to override server role colors on the client.


------

## Setting up BeautifulDiscord

The first step is to set up [BeautifulDiscord](https://github.com/leovoel/BeautifulDiscord), the CSS injector that makes this possible.

1. The first thing you'll want to do is install Python.
  - _Note: Ensure Python is added to your path and that you install it with Pip!_

2. Next, you'll want to use Pip to install the BeautifulDiscord package like so.
{% highlight console %}python3 -m pip install -U https://github.com/leovoel/BeautifulDiscord/archive/master.zip{% endhighlight %}

3. Having done this, you can now simply type `beautifuldicsord` to launch it and generate your custom CSS file! Once you do this you can launch Discord normally, even after restarts, presumably until Discord gets updated again.

## Using your custom CSS

Once you generate your custom css file the tool, you'll need to add entries to override the default role colors.
- _Note: You can change the location with `--css <path>`_

For each role, add a block like this:

{% highlight css %}
* {
    --moderator_new: #2ecc71;
}

*[style="color: rgb(255, 105, 97);"] {
    color: var(--moderator_new) !important;
}
li[class^="role"][style="border-color: rgba(255, 105, 97, 0.6);"] {
    border-color: var(--moderator_new) !important;
}
div[class^="roleCircle"][style="background-color: rgb(255, 105, 97);"] {
    background-color: var(--moderator_new) !important;
} {% endhighlight %}

Each `color: rgb(r, g, b)` is the original role color, which you can find by running the Chromium inspector on either the desktop or web versions of Discord with [this](https://developers.google.com/web/tools/chrome-devtools/shortcuts) first block of shortcuts.

## Full Example
Below you will find a full example that I used for a server I belong to.

{% highlight css %}
* {
    --moderator_new: #2ecc71;
    --researcher_new: #0a91f0;
    --modder_new: #9b59b6;
    --contributor_new: #f0c30e;
}

/* Moderator role: */
*[style="color: rgb(255, 105, 97);"] {
    color: var(--moderator_new) !important;
}
li[class^="role"][style="border-color: rgba(255, 105, 97, 0.6);"] {
    border-color: var(--moderator_new) !important;
}
div[class^="roleCircle"][style="background-color: rgb(255, 105, 97);"] {
    background-color: var(--moderator_new) !important;
}

/* Researcher role: */
*[style="color: rgb(119, 158, 203);"] {
    color: var(--researcher_new) !important;
}
li[class^="role"][style="border-color: rgba(119, 158, 203, 0.6);"] {
    border-color: var(--researcher_new) !important;
}
div[class^="roleCircle"][style="background-color: rgb(119, 158, 203);"] {
    background-color: var(--researcher_new) !important;
}

/* Modder role: */
*[style="color: rgb(255, 179, 71);"] {
    color: var(--modder_new) !important;
}
li[class^="role"][style="border-color: rgba(255, 179, 71, 0.6);"] {
    border-color: var(--modder_new) !important;
}
div[class^="roleCircle"][style="background-color: rgb(255, 179, 71);"] {
    background-color: var(--modder_new) !important;
}

/* Contributor role: */
*[style="color: rgb(‎119, 221, 119);"] {
    color: var(--contributor_new) !important;
}
li[class^="role"][style="border-color: rgba(‎119, 221, 119, 0.6);"] {
    border-color: var(--contributor_new) !important;
}
div[class^="roleCircle"][style="background-color: rgb(‎119, 221, 119);"] {
    background-color: var(--contributor_new) !important;
} {% endhighlight %}