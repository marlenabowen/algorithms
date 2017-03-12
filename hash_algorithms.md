#### 1. Write a function that returns the keys of a hash in an array.

```
function keys_of(hash) {
  array = []
  hash.each do |key, value|
    array.push(key)
  end
  return array
}
```

#### 2. Write a function that returns the values of a hash in an array.

```
function values_of(hash) {
  array = []
  hash.each do |key, value|
    array.push(value)
  end
  return array
}
```

#### 3. Write a function that returns true if a given hash contains a specific key.

```
function includes_key(hash, key_to_find) {
  hash.each do |key, value|
    if key == key_to_find
      return true
    end
  end
  return false
}
```

#### 4. Write a function that returns true if a given hash contains a specific value.

```
function includes_value(hash, value_to_find) {
  hash.each do |key, value|
    if value == value_to_find
      return true
    end
  end
  return false
}
```

#### 5. Write a function that returns how many of a each value are in an array.

```
function count(array) {
  hash = {}
  array.each do |value|
    hash[value] += 1
  end
  return hash
}
```

#### 6. Write a function that turns an array into a hash. Assume your arrays will always have an even number of elements.

```
function to_hash(array) {
  length = 0
  array.each do |element|
    length = length + 1
  end

  index = 0
  hash = {}
  array.each do |element|
    if index < length
      key = array[index]
      hash[key] = array[index + 1]
    end
    index = index + 2
  end
  return hash
}
```

#### 7. Write a function that turns a hash into an array.

```
function to_array(hash) {
  array = []
  hash.each do |key, value|
    array.push(key, value)
  end
  return array
}
```

#### 8. Write a function that returns the keys and values for the keys that are passed in.

```
function slice(hash, keys) {
  new_hash = {}
  keys.each do |key|
    new_hash[key] = hash[key]
  end
  return new_hash
}
```

#### 9. Write a function that returns the keys and values that are not the keys that are passed in.

```
function delete(hash, keys) {
  keys.each do |key|
    hash[key] = nil
  end

  new_hash = {}
  hash.each do |key, value|
    if value != nil
      new_hash[key] = value
    end
  end
  return new_hash
}
```

#### 10. Write a function that merges two hashes

```
function merge(hash_a, hash_b) {
  hash_b.each do |key, value|
    hash_a[key] = value
  end
  return hash_a
}
```

#### 11. Write a function that merges two hashes but sums the values instead of overwriting them. Assume all values received will be integers

```
function sum_merge(hash_a, hash_b) {
  hash_a.each do |key, value|
    if hash_b[key]
      hash_b[key] += value
    else
      hash_b[key] = value
    end
  end
  return hash_b
}
```
