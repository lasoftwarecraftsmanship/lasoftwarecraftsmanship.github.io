---
layout: page
title: Clean Code Checklist
permalink: /clean-code-checklist/
---

Naming things
---------
{% include checkmark.html %} **Name reveals intent** - does the name of the variable, function, or class tell you why it exists, what it does, and how it's used?

{% include checkmark.html %} **Avoid mental mapping** - generally write a name that matches what it's supposed to do, and avoid single digit variable names.

{% include checkmark.html %} **Avoid verbs in class names** - because...

{% include checkmark.html %} **Method naming** - methods should have verb or verb phrase names

Functions
----
{% include checkmark.html %} **What does the function do?** - a function should either (1) do something or (2) answer a question -- not do *both* (1) and (2)

{% include checkmark.html %} **Function size** - rule of thumb might be that more than twenty lines is too long.

{% include checkmark.html %} **Do one thing** ... what else to say?

{% include checkmark.html %} **Indent levels** - more than two indent levels, and it might be too big.

{% include checkmark.html %} **Stick to one level of abstraction** - try not to mix high and low level things in the same function.

{% include checkmark.html %} **Follow the *step down* rule** - organize the class or file to start with the highest level of abstraction and then descend into lower levels of abstraction.

{% include checkmark.html %} **Fewest possible number of function arguments** - zero arguments is best, one argument is good, two arguments and you're getting too complex, three or more arguments... ugh. Why? Lots of reasons, but increased complexity to comprehend the function and complexity in unit testing might be of the strongest.

{% include checkmark.html %} **Avoid side effects** - if your function is doing more than the name suggests (e.g., updating instance variables that nobody expected), then you might consider refactoring. *Or just use an immutable language...*

{% include checkmark.html %} **Avoid output arguments** - e.g., return values should generally be the result of an operation, not a transformation -- better would be to have a method that changes the state of its own object.

Comments
---
//TODO

Formatting
---
//TODO

Credits
---
Original structure and concepts from Uncle Bob Martin's [Clean Code](http://www.amazon.com/Clean-Code-Handbook-Software-Craftsmanship-ebook/dp/B001GSTOAM/)

Additional insight from the <i class="fa fa-calendar"></i> [Los Angeles Software Craftsmanship community](http://www.meetup.com/LA-Software-Craftsmanship/).
