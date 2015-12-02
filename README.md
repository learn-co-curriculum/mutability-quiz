# Quiz: Understanding Mutability

## Objectives

1. Strengthen your understanding of method scopes.
2. Strengthen your understanding of mutability in Ruby.

???

# Mutability Challenge

?: We have the following method that takes in an argument of an array and a string:

```ruby
def quiz_method(array, object)
	array << object
end
```

If we call the method in the following manner:

```ruby
array = ["hi", "there"]

quiz_method(array, "quizmaster")
```

What is the variable `array` now equal to?

( )`["hi", "there"]` (X)`["hi", "there", "quizmaster"]`

?: If we execute the same method in the following manner:

```ruby
array = [1, 2, 3]
quiz_method(array, 4)
```

What is the `array` variable now equal to?

(X)`[1, 2, 3, 4]` ( )`[1, 2, 3]`

?: If we perform the following:

```ruby
string = "hi there "
string << "quizmaster!"
```
What is the value of `string`?

( )`"hi there"` (X)`"hi there quizmaster!"`

?: What is the return value of the following method call?

```ruby
array = [1, 2, 3, 4]
array.each do |num|
	num * 2
end
```

(X)`[1, 2, 3, 4]` ( )`[2, 4, 6, 8]`

?: Below we have a method that accepts two arguments of two numbers:

```ruby
def change_the_number(num1, num2)
	num1 = num1 + num2
end
```

If we call it in the following way: 

```ruby
number_one = 5
number_two = 3
change_the_number(number_one, number_two)
```

What is the value of `number_one`?

(X)`5` ( )`8`

???















<a href='https://learn.co/lessons/mutability-quiz' data-visibility='hidden'>View this lesson on Learn.co</a>
