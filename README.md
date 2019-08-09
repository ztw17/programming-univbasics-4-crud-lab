# Array Lab: Create, Retrieve, Update, Delete

## Learning Goals

- Create a new `Array` that contains data as well as a new `Array` that is empty
- Add an element to the end of an `Array`
- Add an element to the front of an `Array`
- Remove an element from the front of an `Array`
- Remove an element from the end of an `Array`
- Retrieve data from a specific `Array` index

## Introduction

In this lab, you will create `Array`s, add data to `Array`s, remove data from `Array`s
and retrieve data from `Array`s.

We will be coding the solutions for each of the above tasks in the body of a
method. In `lib/array_crud.rb` we've defined a series of methods for you, each
of which is responsible for one of the tasks above.

Let's go through the first challenge together.

## `#create_an_empty_array`

Let's run our test suite to get started. Run the tests one at a time with the
`learn --fail-fast` command in your terminal.

If we do so, we'll see our first failure:

![](http://readme-pics.s3.amazonaws.com/Screen%20Shot%202015-10-26%20at%202.05.07%20PM.png)

Our test is telling us that we are expected to code the content of our
`#create_an_empty_array` method such that a new, empty `Array` is created and
returned. Our test `expected` an empty `Array`, `[]`, but got `nil`.

Open up `lib/array_crud.rb` and check out the `#create_an_empty_array` method.
It's empty! Let's write the code that will get the test passing.

We'll use the literal constructor to make a new `Array` with nothing in it:

```ruby
def create_an_empty_array
  []
end
```

Run the test suite again and we should be passing that first test.

## `#create_an_array`

This method should use the literal constructor to create a new `Array`, just like
we did above. This time, however, create an `Array` that contains four elements.
The four elements can be any elements of your choosing, as long as there are
only four of them.

## `#add_element_to_end_of_array`

This method takes in two arguments, an `Array` and the element we want to add to
it. Use the `<<` (shovel) method or the `#push` method to add that element to
the end of the new `Array`.

## `#add_element_to_start_of_array`

This method takes in two arguments, an `Array` and the element we want to add to
it. Use the `#unshift` method to add that element to the start of that `Array`.

## `#remove_element_from_end_of_array`

This method takes in one argument, the `Array` on which we want to operate. Use
the `#pop` method to remove the last item from the `Array`.

## `#remove_element_from_start_of_array`

This method takes in one argument, the `Array` on which we want to operate. Use
the `#shift` method to remove the first item from the `Array`.

## `#retrieve_element_from_index`

This method takes in two arguments, an `Array` and the index number whose element
we want to retrieve. Use the `[]`, bracket method, to return the element stored
at that index number of the given `Array`.

## `#retrieve_first_element_from_array`

This method takes in one argument, the `Array` from which we want to retrieve an
element. Use `[]` notation to return the value stored at the first index of the
`Array`. Remember that `Array`s are zero-indexed. This means that the first index
number is `0` and it counts up from there. So, the first element of an `Array` is
stored at index `0`.

## `#retrieve_last_element_from_array`

This method takes in one argument, the `Array` from which we want to retrieve an
element. There are a number of ways to do this, but we recommend using the `[]`
method with the following hint:

The last element of an `Array` is considered to be stored at an index of `-1`.

## Conclusion

Congratulations! You just completed learning how to work with create, retrieve,
update, and delete `Array` operations using simple operations provided to us in
Ruby.
