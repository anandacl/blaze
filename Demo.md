---
title: "Demo"
description: "Connect your identity provider to Document360 and map users to reader groups."
---

# An h1 header Change from Git Anand changed

Paragraphs are separated by a blank line.
 
2nd paragraph. *Italic*, **bold**, and `monospace`. Itemized lists
look like:
 
  * this one.
  * that one - changed
  * the other one Gone the other one Done

1) test - changed
2) test 2 - second
3) test 3

Note that --- not considering the asterisk --- the actual text
content starts at 4-columns in.

* new this one. GIT
* new that one - changed
* new the other one Gone the other one Done

> Block quotes are
> written like so.
>
> They can span multiple paragraphs,
> if you like.
 
Use 3 dashes for an em-dash. Use 2 dashes for ranges (ex., "it's all
in chapters 12--14"). Three dots ... will be converted to an ellipsis.
Unicode is supported. ☺

## An h2 header Changed

Here's a numbered list:
 
1. first item
2. second item
3. third item
 
Note again how the actual text starts at 4 columns in (4 characters
from the left side). Here's a code sample:

```text
# Let me re-iterate ...
for i in 1 .. 10 { do-something(i) }
```

In ordinary Markdown that sample is a 4-space indented block. MDX does not support
indented code blocks at all -- indentation is reserved for JSX nesting -- so it is
fenced here instead. Delimited blocks work everywhere and are the safer habit:
 
~~~
define foobar() {
    print "Welcome to flavor country!";
}
~~~
 
(which makes copying & pasting easier). You can optionally mark the
delimited block for Pandoc to syntax highlight it:
 
~~~python
import time
# Quick, count to ten!
for i in range(10):
    # (but not *too* quick)
    time.sleep(0.5)
    print i
~~~
 
 
### An h3 header ###
 
Now a nested list:
 
1. First, get these ingredients:
 
      * carrots
      * celery
      * lentils
 
2. Boil some water.
 
3. Dump everything in the pot and follow
    this algorithm:

    ```text
    find wooden spoon
    uncover pot
    stir
    cover pot
    balance wooden spoon precariously on pot handle
    wait 10 minutes
    goto first step (or shut off burner when done)
    ```

    Do not bump wooden spoon or it will fall.
