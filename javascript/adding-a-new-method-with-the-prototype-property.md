# Adding A New Method With The Prototype Property

Let's say we have a `Class` constructor function, and we want to add a new method to it:

```javascript
function Class(courseTitle, courseNumber, instructor) {
  this.courseTitle = courseTitle;
  this.courseNumber = courseNumber;
  this.instructor = instructor;
}
```
We can do this with the `prototype` property that JavaScript gives us when we create a function.

```javascript
Class.prototype.listInstructor = function() {
  return this.instructor;
};
```
Now, every class we create with our `Class` constructor will have a `listInstructor` method to go along with it.
