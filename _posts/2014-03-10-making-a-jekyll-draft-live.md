---
layout: post
title: "Converting a Jekyll post from draft to live"
category : lessons
tags : [study, jekyll]
---
{% include JB/setup %}

I recently created a jekyll draft, and have reviewed the content in draft mode locally by running `jekyll serve --draft`.

But now that I'm ready to publish the content, what's the best way to convert a jekyll draft to a live post? There has to be a better way than renaming and moving the file to the posts folder.

One way that is better to give Jekyll his butler, [Mr. Poole][1]. Mr. Poole is primarily a command-line application, and it allows you to post, draft, publish, and unpublish.

Check it out here: [https://github.com/mmcclimon/mr_poole] [1]. It downloads and installs from the command line, and documentation is available in the repo.

This post was originally created manually, but I published it live using the following command from Mr. Poole:

`poole publish _drafts/making-a-jekyll-draft-live.md`

[1]: https://github.com/mmcclimon/mr_poole