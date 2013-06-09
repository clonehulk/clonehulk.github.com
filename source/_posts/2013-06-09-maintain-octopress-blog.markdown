---
layout: post
title: "Maintain Octopress blog"
date: 2013-06-09 01:27
comments: true
categories: 
---
This notes is about how to maintain Octopress blog in Github.
<!—more—>
1. Clone your blog from Github
    <pre><code>git clone git@github.com:clonehulk/clonehulk.github.com.git</code></pre>

2. Checkout the source branch:
    <pre><code>git checkout source</code></pre>

3. Set the relationship between your local folder and Github pages:
    <pre><code>rake setup_github_pages</code></pre>
    And follow the message to enter some information.

4. Update your latest blog source code:
	<pre><code>git pull origin source  # update the local source branch</code></pre>
    
5. Write new blogs:
    <pre><code>rake new_post["title"]
rake generate
rake preview</code></pre>

6. Commit to Github:
    <pre><code>rake deploy
git add .
git commit -am 'comment'
git push origin source</code></pre>

Want to config your Octopress? Try this:[Configuring Octopress](http://octopress.org/docs/configuring/).