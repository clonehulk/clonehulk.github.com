---
layout: post
title: "Maintain octopress blog"
date: 2013-06-09 01:27
comments: true
categories: 
---
This notes is about how to maintain Octopress blog in Github.

1. Clone your blog from Github
    <pre><code>
git clone git@github.com:clonehulk/clonehulk.github.com.git
    </code></pre>
2. Checkout the source branch:
    <pre><code>
git checkout source
    </code></pre>
3. Set the relationship between your local folder and Github pages:
    <pre><code>
rake setup_github_pages
    </code></pre>
    And follow the message to enter some information
4. Write a new blog
    <pre><code>
rake new_post["title"]
rake generate
rake preview
    </code></pre>
5. Update to Github
    <pre><code>
rake deploy
git add .
git commit -am 'comment'
git push origin source
    </code></pre>
