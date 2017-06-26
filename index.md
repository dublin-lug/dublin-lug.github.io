---
layout: default
---

# $ cat /proc/about
{:id="about"}

**TODO** description about dublug

# $ find /home/dublug -iname "contact"
{:id="contact"}
Join us via:
* [#dublug](http://webchat.freenode.net/?channels=dublug&uio=d4) channel on irc.freenode.net
  (click on the link or use IRC client such as hexchat).
* our [meetup](https://www.meetup.com/Dublin-Linux-User-Group/) page.
* our [mailing list](https://groups.google.com/forum/#!forum/dublin-lug).

# $ ps -aux|grep news
{:id="posts"}

<ul>
{% for post in site.posts %}
<li><a href="{{ post.url }}" title="{{ post.description }}">{{ post.title }}</a></li>
{% endfor %}
</ul>
