---
layout: post
title: "Maintain Octopress blog"
date: 2013-06-09 01:27
comments: true
categories: 
---
This notes is about how to maintain Octopress blog in Github.
<!-- more -->
1. Clone your blog from Github
{% codeblock lang:bash %}
git clone git@github.com:clonehulk/clonehulk.github.com.git
{% endcodeblock %}

2. Checkout the source branch:
{% codeblock lang:bash %}
git checkout source
{% endcodeblock %}

3. Set the relationship between your local folder and Github pages:
{% codeblock lang:bash %}
rake setup_github_pages
{% endcodeblock %}
    And follow the message to enter some information.

4. Update your latest blog source code:
{% codeblock lang:bash %}
git pull origin source  # update the local source branch
{% endcodeblock %}

5. Write new blogs:
{% codeblock lang:bash %}
rake new_post["title"]
rake generate
rake preview
{% endcodeblock %}

6. Commit to Github:
{% codeblock lang:bash %}
rake deploy
git add .
git commit -am 'comment'
git push origin source
{% endcodeblock %}

Want to config your Octopress? Try this:[Configuring Octopress](http://octopress.org/docs/configuring/).
