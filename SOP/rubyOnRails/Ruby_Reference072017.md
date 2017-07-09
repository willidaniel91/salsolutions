#### Ruby Language Reference Guide

---

#### Helpful Methods

`.class`: To find out what class the object belongs to.

Example:
```Ruby
Variable_name.class
```

`.methods`: To find out methods available to an object.

Example:
```Ruby
object_name.methods
```

`gets.chomp`: To get input from the command line.

```Ruby
gets.chomp
```

* To assign the input to a variable so it can be referenced later on:
  ```Ruby
  variablename = gets.chomp
  ```

`object.odd?`: returns boolean value true if the object is odd.

Example:
```Ruby
22.odd?
```
`object.even?`: returns boolean value true if the object is even.

Example:
```Ruby
22.even?
```

`rand(int)`: generate a random number between 0 and less than *int*:

Example:
```Ruby
rand(10)
```

##### Type Conversion
`.to_i`: to convert an string object to integer.

`.to_s`: to convert an object to a string.

`to_f`: to convert an object to a float.





---

#### Guides

**String interpolation:** use #{} inside a string to interpolate variables into the string.

(has to be within double quotes)
```Ruby
name = "Andrew"

"My name is #{name}"
```

```Ruby
# This will not work due to the use of single quotes
name = "Andrew"

'My name is #{name}'
```

**Escape Symbol:**
To escape the evaluation of #{variablename} within a String, prepent with a \.

```Ruby
\#{variablename}
```
