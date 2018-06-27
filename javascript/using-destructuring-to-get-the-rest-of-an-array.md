# Using Destructuring To Get The Rest Of An Array

Let's say we have an array of states that we're working with and we only care about the "sunshine" state.

```javascript
const states = ['Florida', 'Ohio', 'California', 'New York', 'Texas'];

```

In ES6, we can grab the first value and then destructure the rest of our `states` array into a variable.


```bash
> const states = ['FL', 'OH', 'TX', 'AL', 'MA'];
undefined
> const [sunshine, ...others] = states;
undefined
> sunshine
'FL'
> others
[ 'OH', 'TX', 'AL', 'MA' ]

```

The `...` syntax is basically saying give me the rest of the elements in our states array and assign it to the `others` variable.
