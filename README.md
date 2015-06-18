# Quiz: Understanding Mutability

## Objectives

1. Strengthen your understanding of method scopes
2. Strengthen your understanding of mutability in Ruby

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

what is the variable, `array`, now equal to?

( )`["hi", "there"]` (X)`["hi", "there", "quizmaster"]`

?: If we execute the same method in the following manner:

```ruby
array = [1, 2, 3]
quiz_method(array, 4)
```

What is the `array` variable now equal to?

(X)`[1, 2, 3, 4]` ( )`[1, 2, 3]`

?: What is the return value of the following method call?

```ruby
array = ["hi", "there", "quizmaster"]
array.each do |word|
	word << "!"
end
```

( )`["hi", "there", "quizmaster"]` (X)["hi!", "there!", "quizmaster!"]

?: What is the return value of the following method call?

```ruby
array = [1, 2, 3, 4]
array.each do |num|
	num * 2
end
```

(X)`[1, 2, 3, 4]` ( )`[2, 4, 6, 8]`


???














