# Why I don't like to create HTML with templates

I feel lonely.

I feel lonely because I think I am the only software developer on planet earth
does not like to create HTML with templates.

Context: This is about creating HTML on the backend.

I like [format_html()](https://docs.djangoproject.com/en/dev/ref/utils/#django.utils.html.format_html) which
is a small helper to create [safestrings](https://docs.djangoproject.com/en/dev/ref/utils/#module-django.utils.safestring) with Django/Python.

Most developers like to seperate code and HTML. They use Python/Ruby/Node... for the code and some kind of template language to create HTML.

Most developers use spererate files: One for code, one for the template.

I worked with collegues who wrote nice redundancy-free Python code.

But as soon as they worked with templates the copy+paste fun began. 

Copy-and-pasting code is not done. But copy-and-pasting templates is considered ok.

Grrr.

Why? 

I think creating a utility method in your favorite programming language is easy. Most
developers will do it, instead of copy-and-pasting the same code again and again.

But creating a re-usable method which gets used in the template .... That's a bit harder, 
and thus copy+paste.

Let's embrace HTML fragments. 

I think many people still have an outdated perspective on HTML. Most people think HTML always starts with a `<html> tag, then a `<head>` tag,
then a `<body>` tag. If you think like this, then it makes sense that you need some kind of template and template language to create such a construct.
  
I think about HTML fragments. I create one HTML fragment with one method written in my prefered backend language. This is easy to develop and easy to test.
  
Errors in templates give me a super ugly stacktrace. Each time it is difficult for me to see what the root cause it.
  
It is not impossible, but debugging errors in templates is much harder than debugging my favorite backend language.

While writing code and running the tests I often insert `assert 0, value_which_I_want_to_see`. This gives my a nice stacktrace
and shows me the value which I want to inspect. That's faster than starting the debugger. Is this possible with a template language?
  
I don't use tailwind, but many seem to like it, because it helps you to keep things in one place, in one file.
  
There is a related article of Carson Gross [Locality of Behaviour](https://htmx.org/essays/locality-of-behaviour/).  

So maybe I am not alone.
  
... to be continued.


# I love feedback

You found a mistake or you have an idea how to improve this page? Please create an Github issue.

# Related

[Thomas Working-out-Loud](//github.com/guettli/wol)

