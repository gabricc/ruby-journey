# Ruby Integers

This document covers the basics of working with integers in Ruby.

## Number Formatting
Ruby allows you to use underscores in numbers to make them more readable:
```ruby
2_000_000  # => 2000000
2_000_000 * 2  # => 4000000
```

## Basic Arithmetic Operations
```ruby
8 / 2   # => 4    (Division)
20 % 6  # => 2    (Modulo - returns remainder)
```

### Integer vs Float Division
```ruby
10 / 3    # => 3         (Integer division)
10 / 3.0  # => 3.3333333333333335  (Float division)
10 / 3.to_f  # => 3.3333333333333335  (Converting to float)
```

## Comparison Operators
```ruby
3 > 8   # => false
3 < 8   # => true
3 == 3  # => true
3 != 3  # => false
7 <= 4  # => false
```

### Spaceship Operator (<=>)
The spaceship operator returns:
- 1 if left is greater
- -1 if right is greater
- 0 if equal

```ruby
7 <=> 4  # => 1
7 <=> 8  # => -1
7 <=> 7  # => 0
```

## Useful Integer Methods
```ruby
-5.abs    # => 5     (Absolute value)
5.even?   # => false (Check if even)
4.even?   # => true
12.digits # => [2, 1] (Convert to array of digits)
123.digits # => [3, 2, 1]
```

## Iteration with Integers
Using `times`:
```ruby
# Basic iteration
5.times { puts "hello, world" }

# Iteration with index
5.times do |n| 
  puts "hello, world #{n}"
end
```
Output:
```
hello, world 0
hello, world 1
hello, world 2
hello, world 3
hello, world 4
```

## Floating Point Numbers (Floats)
Floats are numbers with decimal points. Ruby provides several useful methods for working with floats:

```ruby
# Rounding and Ceiling/Floor
4.5.ceil   # => 5    (Round up to nearest integer)
4.5.floor  # => 4    (Round down to nearest integer)
4.5.round  # => 5    (Round to nearest integer)
4.4.round  # => 4
4.1.ceil   # => 5    (Always rounds up)

# Number Properties
-1.positive?  # => false  (Check if number is positive)
```

Floats are commonly used in calculations requiring decimal precision, though be aware that floating-point arithmetic can sometimes lead to small rounding errors due to how computers represent decimal numbers internally.
