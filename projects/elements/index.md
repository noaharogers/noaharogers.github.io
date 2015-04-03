---
layout: posts
name: Noah Rogers
title: Basic HTML Elements
date: June 18, 2014
---
<p>When using HTML elements to create your website it is important to know which of the elements you are working with are block or inline and how they differ from one another.</p>

<p>There are three main types of elements. Virtually every item you see on an internet website falls in to one of the following categories: Inline, Inline-Block, and Block. Let's go ahead and get started.</p>

<h2>Inline Elements</h2>

<p>The first example is Inline elemtns. Inline elements are very common. Here a few common examples of inline elements, and how you may use them:</p>

<p><strong>span</strong> classes can be used in a variety of different ways. On this page I have used a span to add a box around various HTML and CSS elements I mention in this post because it is important to distinguish code from normal text.</p>

<script src="https://gist.github.com/Treydor/64bdb243a8a7d1193f31.js"></script>

<div class="box example">
  <div class="container">
    <p>This is a <span class="example-element inline">span</span>. It will remain inline.</p>
  </div>
</div>

<p>Below are some more common inline elements. Throughout this project I&rsquo;ll do my best to first demonstrate them in HTML, followed by an example of how they will look in browser.</p>

<script src="https://gist.github.com/Treydor/cf56a04c2134e3383e77.js"></script>

<div class="box example">
  <div class="container">
    <p>This will be <strong>bold</strong>.</p>
    <p>This will be <em>italic</em>.</p>
    <p>This <a href="http://www.google.com" target="_blank">link</a> will take you to Google.</p>
  </div>
</div>

<p>Inline elements are just that, in <em>the</em> line. As you can see above, these inline elements stay in the same line they are used. Because these elements are inline, they can have their margin and padding changed, but height and width will be ignored because the inline element is determined by the property it is wrapped around in the HTML.</p>

<h3>So, what did we learn about inline?</h3>
<ul>
  <li>Does not force a line break when used.</li>
  <li>Commonly used to create a link, bold, italicize or create boxes around words and sentences.</li>
  <li>Margin and padding can be changed, but the height and width properties will be ignored.</li>
  <li>Using a block element inside of inline elements is not a good thing. If you want a block element to behave like an inline element continue on to the next section.</li>
</ul>

<h2>Inline-Block Elements</h2>

<p>Inline-Block borrow aspects from both <inline</code> and block. This property can be used in your CSS by adding a <code>display: inline</code>, <code>display: inline-block</code> or <code>display: block</code> property to your element.</p>

<p>Below are a few division elements that use a <code>display: inline-block</code> property:</p>

<script src="https://gist.github.com/Treydor/4329fe9a6ed92a74c1f3.js"></script>

<div class="box example center">
  <div class="container">
    <div class="example-element inline-block">inline-block</div>
    <div class="example-element inline-block">inline-block</div>
    <div class="example-element inline-block">inline-block</div>
  </div>
</div>

<p>There are a few advantages of using inline-block as you can set the height, width, padding and margins on this property while still allowing it to remain inline.</p>

<p>One of the biggest advantages of inline-block is the ability to use the <code>vertical-align</code> property. This property can be written in to your CSS as demonstrated below:</p>

<script src="https://gist.github.com/Treydor/8e29d5b283eaca8da999.js"></script>

<p>To make the example clear I styled one of the elements by coloring it grey and giving it some height. Below are the three <code>vertical-align:</code> properties:</p>

<div class="example box center">
  <div class="container">
    <div class="example-element inline-block large">top</div>
    <div class="example-element inline-block valign-top">inline-block</div>
  </div>

  <div class="container">
    <div class="example-element inline-block large">middle</div>
    <div class="example-element inline-block valign-middle">inline-block</div>
  </div>

  <div class="container">
    <div class="example-element inline-block large">bottom</div>
    <div class="example-element inline-block valign-bottom">inline-block</div>
  </div>
</div>

<h3>A few things to remember about inline-block...</h3>
<ul>
  <li>Inline-Block elements allow you to set a height, width, margin and padding properties, while still allowing the element to remain inline.</li>
  <li>Inline-Block elements may make use of the vertical-align property as demonstrated above.</li>
</ul>

<h2>Block Elements</h2>

<p>Like inline, there are a variety of block elements. Below are just a few of some of the more commonly used block elements as well as some examples of how they may be used</p>

<p>We will start with one of the most common, if not the most common block element, division.</p>

<p>A division, or div, is an extremely common block element that you will surely use on your page. The example below is shows exactly how a division works in the browser.</p>

<script src="https://gist.github.com/Treydor/82f82b8d8752eb3e43ad.js"></script>

<div class="example box">
  <div class="container">
    <div class="example-element block">div</div>
    <div class="example-element block">div</div>
    <div class="example-element block">div</div>
  </div>
</div>

<p>You can see that this element takes up all the space that is available from left-right. A block elements will always force a line break after them.</p>

<p>As you can imagine div elements have numerous uses. More commonly, these elements can be used as containers for just about anything. So you may be asking yourself <q>what are some real world examples of block elements working with one another?</q> Well you are in luck! Below are a few <strong>very</strong> common example of block elements in their most basic forms.

<script src="https://gist.github.com/Treydor/bf39ca2026c03eee1f99.js"></script>

<div class="example box">
  <div class="container">
    <h2>Example Header</h2>
    <p>This is an example of how a paragraph works in relation to a header.</p>
  </div>
</div>

<p>Here you can see our example header automatically force a line break when it is used. This is a block element working exactly as intended.</p>

<p>Other block elements include ol, ul and li elements. Typically used for creating lists, these elements and how they function are demonstrated below:</p>

<script src="https://gist.github.com/Treydor/62da44cfe3aaff1fa2dc.js"></script>

<div class="example box">
  <div class="container">
    <ul>
      <li>Item 1</li>
      <li>Item 2</li>
      <li>Item 3</li>
      <li>Item 4</li>
    </ul>
  </div>
</div>

<p>As you can see from above, these list elements can be extremely useful for many reasons when creating a layout, a system for blog posts, or creating a general list.</p>

<h3>Let&rsquo;s recap block elements</h3>
<ul>
  <li>
    Unless otherwise specified, block elements start on a new line and will always force a line break when being used.
  </li>
  <li>
    If the width property is not set, block elements will fill the entire space available from left to right.
  </li>
  <li>
    Block elements can contain inline elements and are frequently used to "<a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Block-level_elements" target="_blank">create larger structures</a>" than inline elements.
  </li>
  <li>
    Lastly, block elements can have margins, padding, height and width, but, unlike inline-block elements, ignore the vertical-align property.
  </li>
</ul>

<h2>References</h2>
<ul>
  <li>
    Block/Inline-level elements <a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Block-level_elements" target="_blank">Mozilla Developer Network</a>
  </li>
  <li>
    Difference between block and inline (CSS) <a href="http://www.impressivewebs.com/difference-block-inline-css/" target="_blank">Impressive Webs</a>
  </li>
  <li>
    Getting to Know HTML <a href="http://learn.shayhowe.com/html-css/getting-to-know-html/" target="_blank">learn.shayhowe.com</a>
  </li>
</ul>