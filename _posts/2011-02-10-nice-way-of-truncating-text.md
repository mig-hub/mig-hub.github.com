---
layout: main
permalink: pretty
---

There are dozens of ways of truncating text. We don't always have the same needs, so let me tell you that this way I'm gonna show you is not THE perfect way. It is just one I like because it does quite a good job and it uses Regex, which means that it can be done in many languages.

Basicaly it truncates your string without cutting the last word and add `...` when needed. Here is the selection regex:

    /^(.{30}\w*).*$/

30 is the character limit. And here is the replacement bit:

    '$1...'

The main default would be that the end of the last word and the 3 dots are not counted in the 30 characters but that is acceptable for a summary function or a `read-more` link.