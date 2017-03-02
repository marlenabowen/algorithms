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
      break
    end
    }
  }
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
  count = 0
  index = nil
  array.each do |element|
    count = count + 1
    if element == value
      index = count -1
      break
    end
  end
  return index
}
```

#### 6. Write a function that doubles an array.

```
function double(array) {
  copy_array = []
  array.each do |element|
    copy_array.push(element)
  end

  copy_array.each do |element|
    array.push(element)
  end
  return array
}
```

# 7. Write a function that returns a list of unique values in an array. Do not use a hash.

```
function unique(array) {

}
```

#### 8. Write a function that returns the element in an array at the given index. Do not use the built-in method for doing this.

```
function value_at_index(array, index) {
  count = 0
  array.each do |element|
    count = count + 1
    if count == index + 1
      return element
      break
    end
  end
}
```

#### 9. Write a function that reverses an array.

```
function reverse(array) {
  count = 0
  array.each do |element|
    count = count + 1
  end

  popped_element = nil
  reversed_array = []
  while count != 0
    popped_element = array.pop()
    reversed_array.push(popped_element)
    count = count - 1
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

  last = nil
  array.each do |element|
    count = count - 1
    if count == 0
      last = element
      break
    end
  end
  return last
}
```

# 11. Write a function that returns the smallest value in an array.

```
function min(array) {

}
```

# 12. Write a function that returns the largest value in an array.

```
function max(array) {

}
```

#### 13. Write a function that takes two arrays, and returns the count of the elements that have the same value in the same position. The given arrays will be of equal length.


```
function count_same_as_value_position(array_a, array_b) {
  length = 0
  array_a.each do |element|
    length = length + 1
  end

  index = 0
  count = 0
  while index <= length
    if array_a[index] == array_b[index]
      count = count + 1
    end
    index + 1
  end
  return count
}
```

#### 14. Write a function that returns true if the array is sorted.

```
function is_sorted(array) {
  count = 0
  sorted = true
  array.each do |element|
    count = count + 1
    if element > array[count]
      sorted = false
      break
    end
  end
  return sorted
}
```

#### 15. Write a function that returns every other element in an array.

```
function every_other(array) {
  count = 0
  index = 0
  new_array = []
  array.each do |element|
    count = count + 1
  end
  while index <= count
    element = array[index]
    new_array.push(element)
    index = index + 2
  }
  return new_array
}
```
