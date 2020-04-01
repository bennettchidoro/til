# Using Partials To Remove Duplication And Cleanup Views

First off, what is a partial? Just think of a partial as a reusable view chunk of code that can be rendered from other views.

Partials always start with and underscore (`_`) and to render a partial, you use the `render` method.

Say we have a `_form.html.erb` partial and we want to use it in another view. All we have to do is render it and pass the name of the partial without the underscore.

`<%= render "form" %>`

By default, `render` looks for the partial in the same directory as the current view template, so you may need to prefix it with a `/` and then the name of the directory where the partial lives. When there's a `/` in the partial name. `render` treats the first part as the directory name.

`<%= render "layouts/header %>"`<br>
`<%= render "layouts/footer"`

The same goes for when you want to cleanup some of your views using partials.
