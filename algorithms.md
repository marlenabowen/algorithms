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
