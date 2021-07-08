---
subheadline: "Univ. assistant"
title:  "Dr."
first: "Stefan"
family: "Schupp"
mail: "name.surname@tuwien.ac.at"
role: "University Assistant"
image:
  thumb: "people_pictures/schupp.png"
  homepage: "people_pictures/schupp.png"
---

I am a post-doctoral researcher at Trust-CPS Group. This page of mine serves as a quick reference for markdown and is based on [this guide](https://www.markdownguide.org/basic-syntax/)


# This is a first-level heading

with some regular content, i.e., paragraph-style.

## A second-level heading: Typesetting

looks like this. We also should observe, that the content floats around the image. I think we may want to put some keywords (e.g., 3-5) for everyone to enforce a fixed style or we can put the image to the left as well. The image is defaulted by me and fixed in the template - if you do not like it, we can remove it, of course.

If you want to start a new paragraph, insert an empty line. Also, I think manual line breaks do have a semantics here, so if we want to have one single paragraph we better not manually break lines.
I did it anyway, just to see what happens (apparently this does not change anything here). By the way, of course you can have __bold__ faced text, also **this** is bold and if you want to have a p**art** of the word bold this is also possible. If you use single asterisks, the text becomes *italic*. Same holds for single bars, but I was told we should _not_ use this for some reason (bad practice - stick to asterisks, also for bold-faced text). __*Of course*__ you can combine both, the shortcut with ***three asterisks*** seems more consistent with the last rule.

By the way, I think famous words should be formatted as a quote
> Im großen Garten der Geometrie kann sich jeder nach seinem Geschmack einen Strauß pflücken. (David Hilbert)

Now that I see it, the spacing before the third heading is weird, if you put a quote directly before it.

### Third-level heading: Lists

where of course we can still put content.

If you need lists, those come in handy:
- 1st item
- 2nd item


I think you can also enumerate:
1. this is the first step
2. this is the second step
1. the numbering in the code does really not matter, apparently
1. see?

By the way, horizontal lines are the new line break. You can use three or more of asterisk, dash or underscore in a separate line to achieve this.

***

#### Code

I am not sure whether needed, but you can put code by indenting by one tab or four spaces, e.g.:

    int main() {
      std::cout << "Hello world" << std::endl;
      return 0;
    }

Afterwards we may continue with regular text. Sometimes I feel like putting inline code: `void*` sometimes are useful.

#### Links

By the way, images and [links](http://www.stefanschupp.de) almost have the same syntax.
Interestingly, if you forget/remove the `https://`-part in the url, the link acts as a local link - we need to test this at some point.

#### Images

Since I like my picture, I will put it again. Rememer to put the full adress until I have figured out how to use relative adresses here.

![Stefans picture](https://trust-cps-group.github.io/images/people_pictures/schupp.png "Look mum, I can add a mouseover text!")

What is really annoying in my opinion are resized images, as there does not seem to exist a nice way of doing this. So instead use html-code, as such:

<img src="https://trust-cps-group.github.io/images/people_pictures/schupp.png" alt="Stefan again" width="100" height="auto">
