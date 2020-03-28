# Embedded Ruby (ERb)

Embedded Ruby or ERB is a templating language that ships with Rails. I like to
think of it as HTML with some Ruby sprinkles.
Erb files end in the `.erb` extension and come in two different flavors.

The first flavor runs the Ruby code and substitutes the result into the template. (Make note of the equal sign). <br>
`<%= %>`

The second flavor runs the Ruby code, but does not substitute the result into the template. <br>
`<% %>`
