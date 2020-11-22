---
title: Creative link styling
date: 2020-11-20 21:00:00 +0100
categories: [Front-End, Styling]
tags: [tips and tricks, css a]
---

<style>
.post-content a.test {
  text-decoration: none !important;
  background-color: transparent !important;
  display: inline-block !important;
  color: inherit !important;
  border-bottom: 2px solid #fc0 !important;
  background-image: linear-gradient(120deg,#fc0,#fc0) !important;
  background-repeat: no-repeat !important;
  background-size: 100% 0 !important;
  background-position: 0 100% !important;
  transition: background-size .125s ease-in !important;
}
.post-content a.test:hover {
    text-decoration: none !important;
    background-size: 100% 100% !important;
    color: #212529 !important;
    cursor: pointer;
}
</style>

It's very nice and simple idea how to present links on the websites. By using `linear-gradient` as a `backgorund-image` and `transition`, which changes `background-size` to the whole its possible hight. To achieve this smooth link background effect, add below code to desired HTML `a` tag class/id.

```css
a {
  text-decoration: none;
  background-color: transparent;
  display: inline-block;
  color: inherit;
  border-bottom: 2px solid #9c0;
  background-image: linear-gradient(120deg,#9c0,#9c0);
  background-repeat: no-repeat;
  background-size: 100% 0;
  background-position: 0 100%;
  transition: background-size .125s ease-in;
}
a:hover {
  text-decoration: none;
  background-size: 100% 100%;
  cursor: pointer;
}
```
Colors and contrast matter not only because of the accesiility but also because of user experience, so play with text and background colors to get good transparency and readability. And here is the working example. <a class="test">Just hover over the link :)</a>.
