# Ruby Strings

This document covers the basics of working with strings in Ruby.

## String Creation and Quotes
Ruby supports both single and double quotes for creating strings. Double quotes allow for escape sequences and string interpolation.

```ruby
# Single quotes
'they said "hello"'  # => "they said \"hello\""

# Double quotes with escape sequences
"they said \"hello\""  # => "they said \"hello\""
puts "they said \"hello\""  # Output: they said "hello"
```

## String Interpolation
Ruby allows you to embed expressions inside strings using `#{...}`. This only works with double-quoted strings.

```ruby
"2 + 2 = #{2+2}"  # => "2 + 2 = 4"
```

## Object-Oriented Nature
In Ruby, everything is an object, including strings:

```ruby
"".class     # => String
"hello".class  # => String
2.class      # => Integer
2.1.class    # => Float
```

## String Methods
Ruby provides many useful methods for string manipulation:

```ruby
# Substituting text
"Hello, world".sub("Hello", "Good morning")  # => "Good morning, world"
```

### Common String Methods (Additional Examples)
- `upcase`: Convert string to uppercase
- `downcase`: Convert string to lowercase
- `capitalize`: Capitalize first letter
- `strip`: Remove leading and trailing whitespace
- `split`: Split string into array
- `length` or `size`: Get string length
