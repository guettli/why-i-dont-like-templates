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


... to be continued.


# I love feedback

You found a mistake or you have an idea how to improve this page? Please create an Github issue.

# Related

[Thomas Working-out-Loud](//github.com/guettli/wol)

