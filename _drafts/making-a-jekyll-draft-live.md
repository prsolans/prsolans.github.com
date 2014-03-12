---
layout: post
title: "Converting a Jekyll post from draft to live"
category : lessons
tags : [study, jekyll]
---
{% include JB/setup %}

_You are a writer_ who has created a jekyll draft, and have reviewed the content in draft mode locally by running `jekyll serve --draft`.

If you are ready to publish the content, how do you convert a jekyll draft to a live post? There has to be a better way than renaming and moving the file to the posts folder.

One way that is better to give Jekyll his butler, [Mr. Poole][1]. Mr. Poole is primarily a command-line application, and it allows you to post, draft, publish, and unpublish.

Check it out here: [https://github.com/mmcclimon/mr_poole] [1]

This post was originally created manually, but I published it live using the following command:

`poole publish _drafts/making-a-jekyll-draft-live.md`

[1]: https://github.com/mmcclimon/mr_poole