---
layout: post
title:  "Horizontal scroll box"
date:   2017-06-17 10:07:39 -0700
categories: Web_Design
---
## Horizontal Scroll box
If you are a Blogger, you have to create horizontal scrolling boxes for showing your codes. It is not easy to setup [SyntaxHighlighter](http://alexgorbatchev.com/SyntaxHighlighter/) or [Prism](http://prismjs.com) for Blogger like WordPress. However you can create beautiful horizontal scroll boxes for codes. In this post I will show you how it becomes possible. Go to your blogger control panel and create a new post. Whenever you want a code snippet you can use following code.
<pre class="line-numbers">
<code class="language-css">
<style>
.divScroll{ 
            white-space: nowrap; 
            overflow-x: scroll;
            font-size:14px;
            height:auto;
            width:auto;
            background-color:#bdbdbd;
        }
</style>
<div class="divScroll">
"Your Code"
</div>
If you have any trouble with these symbols: `<` and `>` use `&lt;` and `&gt;`
