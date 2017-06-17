---
layout: post
title:  "WhatsApp Share and Contact Button"
date:   2017-06-17 10:07:39 -0700
categories: jekyll
---
# Whatsapp Share Button
Nowadays Whatsapp became a powerful messegaing platform. So get in touch with friends and colleagues we are using whatsapp. So Whatsapp has 600 million users in world wide. Ot is not a small number. Nowadays WhatsApp has more number of users than any other social media except facebook. In this post we will discuss how can we create a WhatsApp share button for a Jekyll Website. See the following code.
```markdown
<a href="whatsapp://send?text=The text to share!" data-action="share/whatsapp/share">Share via Whatsapp</a>
```
It will show something like this:
<a href="whatsapp://send?text=The text to share!" data-action="share/whatsapp/share">Share via Whatsapp</a>
Now we want to think how can we use use this as the share button. We know that for our Jekyll website has `site.url`, `base.url` and a `page.url`. We want share the url of post. It usually looks like https://chipprogrammers.github.io/jekyll/2017/06/17/whatsapp-share-and-contact.html. Here https://chipprogrammers.github.io is my `site.url` and /jekyll//2017/06/17/whatsapp-share-and-contact.html is my `page.url`. I have no site.baseurl since I am named my repository in the format `username.github.io`. Now we can see how the code should be written.
```markdown
<a href="whatsapp://send?text=`{{site.url}}{{ page.url }}`" style="position: relative; top: -8px; padding: 3px 8px 3px 8px;color: #fff;font-size: 11px;font-weight: bold;font-family: Helvetica, Arial, sans-serif;background-color: #5bb66f;border-radius: 3px;"><i class="fa fa-whatsapp" aria-hidden="true"></i> Whatsapp</a>
```
This will produce a button like following:<br />
<a href="whatsapp://send?text={{site.url}}{{ page.url }}" style="position: relative; top: -8px; padding: 3px 8px 3px 8px;color: #fff;font-size: 11px;font-weight: bold;font-family: Helvetica, Arial, sans-serif;background-color: #5bb66f;border-radius: 3px;"><i class="fa fa-whatsapp" aria-hidden="true"></i> Whatsapp</a>
