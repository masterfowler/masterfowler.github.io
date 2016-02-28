---
layout: post
title:  "Hello World"
date:   2016-02-28 16:33:39 +1300
categories: Misc
css: helloworld
---

To kick this blog off I thought I'd make a Hello World post. Since learning any new programming language typically begins with making a simple Hello World program this seems appropriate.

This is a simple Hello World program using css animation.

<div class='helloworld-container'>
	<div class='helloworld-box'>
		H
	</div>
	<div class='helloworld-text'>
		ello World!
	</div>
<div>

<br />
<br />

For those interested, here is the code.
<br />
<i>NB: the code can also be found on my codepen <a href="http://codepen.io/masterfowler/pen/BjgdYg">here</a>

<br />
<br />
<b>HTML</b>
{% highlight html %}
<div class='helloworld-container'>
	<div class='helloworld-box'>
		H
	</div>
	<div class='helloworld-text'>
		ello World!
	</div>
<div>
{% endhighlight %}

<b>CSS</b>
{% highlight css %}
.helloworld-container {
  position: relative;
}

.helloworld-text {
  animation: change-color 3s infinite linear;
  left: 24px;
  top: 0px;
  position: absolute;
}

.helloworld-box {
  animation: spin-box 2s infinite linear;
  height: 18px;
  width: 18px;
  background-color: #49DB18;
  position: absolute;
  border: solid 2px #222;
  border-radius: 3px;
  color: #000;
  font-style: bold;
  text-align: center;
  left: 0px;
  top: 0px;
}

@keyframes spin-box {
  25% { transform: rotate(45deg) }
  50% { transform: rotate(-45deg) }
  75% { transform: rotate(-45deg) }
}

@keyframes change-color {
  0% { color: #000 }
  50% { color: #49DB18 }
}
{% endhighlight %}