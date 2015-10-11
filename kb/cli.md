---
layout: page
title: "Useful CLI Commands"
published: true
---
<p>&nbsp;</p>

Display just the HTTP response using `curl` ([ref](http://beerpla.net/2010/06/10/how-to-display-just-the-http-response-code-in-cli-curl/))

{% highlight bash %}
curl -IL example.com
{% endhighlight %}

Find the cause of last shutdown/reboot on <em>Linux</em> ([ref](http://unix.stackexchange.com/a/10351))

{% highlight bash %}
last reboot
last -x | grep shutdown
{% endhighlight %}

Restart Frozen dock in <em>Max OSX</em> ([ref](http://www.maclife.com/article/howtos/how_restart_frozen_dock))

{% highlight bash %}
killall Dock
{% endhighlight %}

Inspect memory hardware in <em>Linux</em>

{% highlight bash %}
sudo lshw -C memory
{% endhighlight %}

Search and replace text in multipe files from command line (<em>Linux</em> and <em>Mac OS</em>)

{% highlight bash %}
find . -type f -name "<FILE_FILTER>" -exec sed -i 's/<SEARCH>/<REPLACE>/g' {} \;
# e.g
find . -type f -name "*.txt" -exec sed -i 's/hello/bye/g' {} \;
{% endhighlight %}

Copy SSH public key to a remote server when `ssh-copy-id` is not present

{% highlight bash %}
cat ~/.ssh/id_rsa.pub | ssh user@host "mkdir -p ~/.ssh; cat >> ~/.ssh/authorized_keys"
{% endhighlight %}


