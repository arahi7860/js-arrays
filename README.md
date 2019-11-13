# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png)  SOFTWARE ENGINEERING IMMERSIVE

# JavaScript Arrays
This is the JavaScript Arrays lesson.

# Objectives
*After this lesson, students will be able to:*
- Understand JavaScript Arrays
- Work with JavaScript Arrays


## Arrays

Unfortunately, strings and numbers are not enough for most programming purposes.
What is needed are collections of data that we can use efficiently, Arrays.

Arrays are great for:

* Storing data
* Enumerating data, i.e. using an index to find them
* Quickly reordering data

Arrays, ultimately, are a data structure that is similar in concept to a list. Each item in an array is called an element, and the collection can contain data of the same or different types. In JavaScript, they can dynamically grow and shrink in size.


```javascript
let friends = ['Moe', 'Larry', 'Curly'];
=> ['Moe', 'Larry', 'Curly']
```

Items in an array are stored in sequential order, and indexed starting at `0` and ending at `length - 1`.

```javascript
// First friend
let firstFriend = friends[0];
 => 'Moe'
// Get the last friend
let lastFriend = friends[2]
=> 'Curly'
```

We can even use strings like arrays:

```javascript
let friend = "bobby bottleservice";
// pick out first character
friend[0]
//=> 'b'
friend.length
```

## Working with Arrays

Using the JavaScript Keyword `new`, is one way of creating arrays:

```javascript
let a = new Array();
=> undefined

a[0] = 'dog';
=> "dog"

a[1] = 'cat';
=> "cat"

a[2] = 'hen';
=> "hen"

a
=> ['dog', 'cat', 'hen']

a.length;
=> 3
```

A more convenient notation is to use an array literal:

```javascript
let a = ['dog', 'cat', 'hen'];

a.length;
=> 3
```

#### Length method

The `length` method works in an interesting way in Javascript. It is always one more than the highest index in the array.

So `array.length` isn't necessarily the number of items in the array. Consider the following:

```javascript
let a = ['dog', 'cat', 'hen'];
a[100] = 'fox';
a.length; // 101
```

**Remember**: the length of the array is one more than the highest index.

#### Getting data from an array

If you query a non-existent array index, you get `undefined`:

```javascript
let a = ['dog', 'cat', 'hen'];

a[90];
=> undefined
```

#### Array Helper Methods

Arrays come with a number of methods. Here's a list of some popular helpers:

> Note: You might want to demonstrate a few of these.

- `a.toString()` - Returns a string with the `toString()` of each element separated by commas.

- `a.pop()` - Removes and returns the last item.

- `a.push(item1, ..., itemN)` - `Push` adds one or more items to the end.

- `a.reverse()` - Reverse the array.

- `a.shift()` - Removes and returns the first item.

- `a.unshift(item)` - Prepends items to the start of the array.

Explore the the [full documentation for array methods](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array) and other helper methods given to you for particular objects.
