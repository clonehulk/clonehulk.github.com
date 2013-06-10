---
layout: post
title: "Ruby on Mac"
date: 2013-06-06 19:07
comments: true
categories: Notes
---
The default version of Ruby on Mac OXS is 1.8.7. But the Ruby Rails needs Ruby 1.9.3 or further. So we need update it.

Here is the notes about updating Ruby on Mac.
<!-- more -->
1. Installing [RVM(Ruby Version Manager)](https://rvm.io/) for upgrading Ruby on OXS:
	{% codeblock lang:bash %}
curl -L get.rvm.io | bash -s stable
	{% endcodeblock %}

2. Using this command to show all the available versions of Ruby.
	{% codeblock lang:ruby %}
rvm list known
	{% endcodeblock %}

3. Installing one particular version, for example:
	{% codeblock lang:ruby %}
rvm install ruby 1.9.3
	{% endcodeblock %}

4. Or if you just want the latest (current) version:
	{% codeblock lang:ruby %}
rvm install current && rvm use current
	{% endcodeblock %}

Please note that don't uninstall the default version of Ruby on Mac.
