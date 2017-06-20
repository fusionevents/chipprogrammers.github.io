---
layout:post
title:  "Digital Clock"
date:   2017-06-20 14:20:39 -0700
categories: Web_Design
---
Today we will discuss about how to create a digital clock on your website. It is little bit easier task. We can use Javascript for this task. Create a file `time.html` on your `_includes` directory. The time.html is looks like this. You can change styles according to your perspective.
```markdown
<center>
<style>
#clock{
 color:#5bb66f;
 display:inline;
} 
</style>
<script>
function digclock()
{
 var d = new Date()
 var t = d.toLocaleTimeString()
 
 document.getElementById("clock").innerHTML = t
}
setInterval(function(){digclock()},1000)
</script>
<font color=#5bb66f>Now: </font><div id="clock">
</div>
```
In the seventeenth line of your code you can see a Now:. The same thing you can see at the footer of this site. If there is no `display:inline;`on the style, the time and Now: displayed on the different lines. The  1 sec. delay is produced using `setInterval(function(){digclock()},1000)` which gives 1000 milli second or 1 sec.delay.
