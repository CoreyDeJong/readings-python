## Django Sass Processor
- django-sass-processor converts `*.scss` or `*.sass` files into `*.css` while rendering templates.
- Refer SASS/SCSS files directly from your sources, instead of referring a compiled CSS file, having to rely on another utility which creates them from SASS/SCSS files, hidden in your source tree.
- Use Django's settings.py for the configuration of paths, box sizes etc., instead of having another SCSS specific file (typically _variables.scss), to hold these.
- Extend your SASS functions by calling Python functions directly out of your Django project.
View SCSS errors directly in the debug console of your Django's development server.
- This Django app provides a templatetag `{% sass_src 'path/to/file.scss' %}`, which can be used instead of the built-in templatetag static.

## Sass
- extension to CSS that can help write more flexible styles
- sass is written in ruby
- Sass lets you use features that don't exist in CSS yet like variables, nesting, mixins, inheritance and other nifty goodies that make writing CSS fun again
- Sass uses the $ symbol to make something a variable
- You can create partial Sass files that contain little snippets of CSS that you can include in other Sass files. This is a great way to modularize your CSS and help keep things easier to maintain.
- modules: use `@use 'base'` in the module file and it will send the data into the base.sass file
-  A mixin lets you make groups of CSS declarations that you want to reuse throughout your site.
- Using @extend lets you share a set of CSS properties from one selector to another.
- Sass has a handful of standard math operators like +, -, *, /, and %