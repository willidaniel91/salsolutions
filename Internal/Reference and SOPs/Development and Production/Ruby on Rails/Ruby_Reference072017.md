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

`.is_a?(class_name)`: Returns a boolean value to tell whether the object is class *class_name*

Example:
```Ruby
"String".is_a?(String) #will return true
```

`.method("method_name")`: get hold of any of its methods as an object.

Example:
```Ruby
next_method_object = 1.method("next")
puts next_method_object.call
```
*this will `.call` the method `.next` and is the same as `1.next` ; it returns the integer 2.

`.ancestors`: List the super classes of the object.

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

#### Commonly Used Array Methods

Some methods you can use on arrays:

`arrayname.empty?`: returns boolean true if array is empty.

`arrayname.include?(itemname)`: returns a boolean true if array contains *itemname*.

`arrayname.reverse`: reverses the order of the array. *(preserves original array)*.

`arrayname.reverse!`: use ! at the end to change the original array.

`arrayname.shuffle`: shuffles array into random order.

`arrayname.push(30)`: append new element 30 to the end array.

`arrayname << 25`: known as shovel operator, << will also append new element to the end of the array.

`arrayname.unshift("someelement")`: add element "some element" to the beginning of the array.

`arrayname.pop`: remove the last element of the array **and return 1**.

`arrayname.uniq`: remove all the duplicates and display (will preserve the original array).

`arrayname.uniq!`: remove all the duplicates in the original array.

`(0..99).to_a.shuffle!`: `(0..99)` creates a range *inclusing 0 and 99* , `.to_a` converts the range to an array, and `.shuffle!` stores the array in random order.

`y.each { |i| puts i }`: loop through an array named y using the `.each` method and print out the value of each element.

do-end block:
```Ruby
names.each do |randomvariablename| # starts the do block

puts "Hello #{randomvariablename}" # executes code for each element

end # ends the do block
```

`y.select { |number| number.odd? }`: selects the value and returns it only if the condition is met.

`p.join("-")`: join the elements of an array with a dash between each element.


#### Commonly Used Hash Methods

`my_details["favcolor"]`: access the value and notify me what favcolor is (assuming the *my_details* hash was previously created).

`myhash = {a: 1, b: 2, c: 3, d: 4}`: create a hash with the key-value pairs.

`myhash[:c]`: access the value for *c*.

`myhash[:d] = 7`: add the key-value pair *d: 7*.

`myhash.delete(:d)`: delete a key, value pair by deleting the key.

`myhash.each { |somekey, somevalue| puts somevalue }`: iterate through a hash using `.each` method and print out value.

`myhash.each { |somekey, somevalue| puts "The key is #{somekey} and the value is #{somevalue}" }`: iterate through a hash using .each method and print out both key and value in friendly format.

`myhash.each { |k, v| myhash.delete(k) if v > 3 }`: iterate through and delete a items from a hash based on a condition (if v > 3).

`myhash.select { |k, v| v.odd? }`: use select method to display items only if value of the item is odd

##### Type Conversion
`.to_i`: to convert an string object to integer.

`.to_s`: to convert an object to a string.

`to_f`: to convert an object to a float.

`.to_a`: to convert an object to an array.



---

#### Guides

**String interpolation:**
use #{} inside a string to interpolate variables into the string.

*(has to be within double quotes)*
```Ruby
name = "Andrew"

"My name is #{name}"
```

```Ruby
name = "Andrew"
# This will not work due to the use of single quotes
'My name is #{name}'
```

**Escape Symbol:**
To escape the evaluation of #{variablename} within a String, prepent with a \.

```Ruby
\#{variablename}
```

**Arrays:**
Arrays can be created by including elements within square brackets.
```Ruby
a = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
```

Arrays are zero-indexed.

```Ruby
a[0]  #will print out 1
```

**Hashes:**
Hashes are like arrays with key-value pairs and can be created in a similar way.
```Ruby
my_details = {'name' => 'Andrew', 'favcolor' => 'red'}
```
*or more simply...*
```Ruby
myhash = {a: 1, b: 2, c: 3, d: 4}
```

---
last edited and verified by Andrew Hunsaker on 9.7.2017
