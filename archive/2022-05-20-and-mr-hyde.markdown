---
layout:	post
title:	"... and Mr. Hyde"
date:		2022-05-19 23:48:50 -0700
tags: day2 jekyll motivation
---
Today felt a lot more productive despite actually spending less time on the computer. It's fascinating how quickly one's mood can change when something substantive or physical is produced. If it wasn't for me researching all this stuff about Liquid and SASS yesterday, then I would have never been able to make real changes on the theme itself. With that being said what was actually learned?

Firstly the most useful thing I learned was how to import custom fonts into my webpage. To do so first download the font on to your computer. I used [Google Fonts](https://fonts.google.com) as my website of choice to find fonts, but any font repository will do.

I then converted the font type to .woff (web open font format) since it is supported by pretty much every browser and is from what I can tell, the de facto when it comes to web-displayed fonts. A good site for this is this [webfont generator](https://www.fontsquirrel.com/tools/webfont-generator) from Font Squirrel.

If you used the above generator it should provide a stylesheet but if not, create a stylesheet that has the following:

```css
@font-face {
    font-family: 'font-name';
    src: url('path/to/font.woff') format('woff');
    font-weight: normal;
    font-style: normal;
}
```

This is necessary so that custom font families can be used. For each custom font face that you want you can use this template to 'import' it into css and have your own desired fonts that are not restricted to the web-safe fonts. In my practice, I simply had a file called custom-fonts.css which had a bunch of these font-face at-rules. That way whenever I wanted to use the font, I would simply write `@import "custom-fonts.css";` at the very top which let me specify the font-family wherever I wanted in my new css document.

## Introspection

Aside from the technical things learned with Jekyll, I also learned that 24 hours a day is not a lot of time. Tomorrow I want to track the hours I spend doing certain tasks and see what my breakdown ends up being. I don't necessarily see things such as videogames or TV as bad things but I do believe that they are simple short term benefits and perhaps I spend a bit too much time on them when I can be cultivating my own knowledge and skills in the long term.

Of course, that is part of this whole project/experiment; I am trying to figure out how to mold my life around The Pursuit and not just quick pleasures.

Goodnight 🌙
