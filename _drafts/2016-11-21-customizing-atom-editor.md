---
ID: 1128
post_title: Customizing Atom Editor
author: miklb
post_date: 2016-11-21 05:41:50
post_excerpt: ""
layout: post
permalink: http://michaelbishop.me/?p=1128
published: false
tags:
  - 'a:3:{i:0;s:11:"development";i:1;s:4:"Atom";i:2;s:12:"productivity";}'
summary:
  - >
    In my never ending quest for a perfect
    text editor, some notes on how I
    customize Atom.io editor.
---
I doubt anyone who writes code for a living or tinkers for that matter hasn't spent more hours than they'd care to admit tweaking their editor of choice. Suffice to say, I'm in that boat all to well.

My current editor of choice is [Atom](http://atom.io). It's open source and more than fits the customization itch.

Aside from deciding on which packages to use (I've
[starred the ones I use](https://atom.io/users/miklb/stars)) the other element I've gone back and forth with is theme &amp; syntax UI. I've long been a fan of both Solarized Light and Dark, but have finally settled on Atom Dark and [Oceanic Next](https://atom.io/themes/oceanic-next). I can also recommend [Oliver Pattison's](https://olivermak.es) [Newbound syntax themes](https://atom.io/users/opattison) My dream font is Operator Mono, but until I can justify the purchase of that, I'm using [Input](http://input.fontbureau.com/info/).

One tweak I just discovered is for adjusting the font size in the panel, or the sidebar. I'd been able to easily make the font larger for code/markdown, but sometimes had to break the readers out to discern what file was what in a nested folder. To the rescue I found `atom-panel.tool-panel` for just that. I'm currently using `1.4em`. Mind you this is on my old 11 inch Air. I've not had as much an issue on the iMac.

Another tweak I've added to my custom `styles.less` file is to italicize attributes. I'm also a fan of italicized comment blocks, which is included in the snippet.

``` sass
atom-text-editor::shadow{
     .entity.other.attribute-name {
         font-style: italic;
     }

     .comment {
       font-style: italic;
     }
 }
```
I'm sure as I expand my development world, (I have a goal to learn python by [Building a Twitterbot](https://miklb.com/building-a-twitterbot) ) I'll continue to tweak Atom, but for now, I'm as close to happy with an editor as I have ever been. Feel free to share with me on Twitter [@miklb](https://twitter.com/miklb) your tips and trick.
<a href="https://brid.gy/publish/twitter"></a>