#### 1. Write a function that returns how many of a specified value is in an array.

```
function count_of(array, value) {
  count = 0
  array.each do |element|
  	if element == value
  		count = count + 1
  	end
  end
  return count
}
```

#### 2. Write a function that returns true if a given array contains an element, false otherwise.

```
function include(array, value) {
  result = false
  array.each do |element|
    if element == value
      result = true
    end
  end
  return result
}
```

#### 3. Write a function that adds numbers in an array.

```
function add_values(array) {
  sum = 0
  array.each do |element|
    sum = sum + element
  end
  return sum
}
```

#### 4. Write a function that removes all occurrences of a certain value from an array.

```
function remove_value(array, value) {
  array_without_value = []
  array.each do |element|
    if element != value
      array_without_value.push(element)
    end
  end
  return array_without_value
}
```

#### 5. Write a function that returns the index an element is at in an array. Return nil if the element is not in the array.

```
function index(array, value) {
  index = 0
  array.each do |element|
    if element == value
      return index
    end
    index = index + 1
  end
}
```

#### 6. Write a function that doubles an array.

```
function double(array) {
  doubled_array = []
  array.each do |element|
    doubled_array.push(element)
  end

  array.each do |element|
    doubled_array.push(element)
  end
  return doubled_array
}
```

#### 7. Write a function that returns a list of unique values in an array. Do not use a hash.

```
function unique(array) {
  unique_array = []
  array.each do |element|
    if !include(unique_array, element)
      unique_array.push(element)
    end
  end
  return unique_array
}
```

#### 8. Write a function that returns the element in an array at the given index. Do not use the built-in method for doing this.

```
function value_at_index(array, index) {
  count = 0
  array.each do |element|
    if count == index
      return element
    end
    count = count + 1
  end
}
```

#### 9. Write a function that reverses an array.

```
function reverse(array) {
  copy_array = []
  array.each do |e|
    copy_array.push(e)
  end

  reversed_array = []
  array.each do |element|
    value = copy_array.pop()
    reversed_array.push(value)
  end
  return reversed_array
}
```

#### 10. Write a function that returns the last element in an array.

```
function last(array) {
  count = 0
  array.each do |element|
    count = count + 1
  end
  return array[count-1]
}
```

#### 11. Write a function that returns the smallest value in an array.

```
function min(array) {
  min = array.first
  array.each do |element|
    if element < min
      min = element
    end
  end
  return min
}
```

#### 12. Write a function that returns the largest value in an array.

```
function max(array) {
  max = array.first
  array.each do |element|
    if element > max
      max = element
    end
  end
  return max
}
```

#### 13. Write a function that takes two arrays, and returns the count of the elements that have the same value in the same position. The given arrays will be of equal length.


```
function count_same_as_value_position(array_a, array_b) {
  index = 0
  count = 0
  array_a.each do |element|
    if element == array_b[index]
      count = count + 1
    end
    index = index + 1
  end
  return count
}
```

#### 14. Write a function that returns true if the array is sorted.

```
function is_sorted(array) {
  index = 1
  sorted = false
  array.each do |element|
    if element < array[index]
      sorted = true
    end
    index = index + 1
  end
  return sorted
}
```

#### 15. Write a function that returns every other element in an array.

```
function every_other(array) {
  index = 0
  new_array = []
  array.each do |element|
    if index % 2 == 0
      new_array.push(element)
    end
    index = index + 1
  end
  return new_array
}
```
