---
layout: post
title: "Ruby on Mac"
date: 2013-06-06 19:07
comments: true
categories: 
---
The default version of Ruby on Mac OXS is 1.8.7. But the Ruby Rails needs Ruby 1.9.3 or further. So we need update it.

Here is the notes about updating Ruby on Mac.
<!-- more -->
1. Installing [RVM(Ruby Version Manager)](https://rvm.io/) for upgrading Ruby on OXS:
    <pre><code>\curl -L get.rvm.io | bash -s stable</code></pre>
3. Using this command to show all the available versions of Ruby.
    <pre><code>rvm list known</code></pre>
4. Installing one particular version, for example:
    <pre><code>rvm install ruby 1.9.3</code></pre>
5. Or if you just want the latest (current) version:
    <pre><code>rvm install current && rvm use current</code></pre>

Please note that don't uninstall the default version of Ruby on Mac.