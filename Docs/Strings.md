# Strings
### Table of Contents
- [string_ext](#string_ext)
- [string_split](#string_strip)
- [string_fill_zero](#string_fill_zero)
- [string_contains](#string_contains)

---
# string_ext
Replace every `{}` with arguments values. The arguments are optional, if you don't pass any argument, the `{}` will not be replaced.

### Syntax
  ```js
  string_ext(string, [*args]);
   ```

| Argument | Type | Description |
| :--- | :---: | :--- |
| string | String | The string to replace |
| args | Any | The arguments to replace the `{}` |
### Returns
  ```js
  String
  ```

### Example
```js
var _str = "Welcome back, {}!";
var _name = "Andrew";
var _str_name = string_ext(_str, _name);

show_debug_message(_str_name);
```

The above code will set the var `_str_name` as an string with the name replaced and the show on console. The result will be `Welcome back, Andrew!`.

---

# string_strip
Returns an array from a string divided on substrings by a separator.

### Syntax
  ```js
  string_strip(string, separator);
  ```

| Argument | Type | Description |
| :--- | :---: | :--- |
| string | String | The string to strip |
| separator | String | The separator to divide the string |
### Returns
  ```js
  Array
  ```

### Example
```js
var _str = "Hello, World!";
var _sep = ", ";
var _str_arr = string_strip(_str, _sep);

show_debug_message(_str_arr);
```

The above code will set the var `_str_arr` as an array with the string divided on substrings and the show on console. The result will be `["Hello", "World!"]`.

---

# string_fill_zero
Returns a string filled with 0's on a chosen side (left or right). The string will be filled with 0's until the string length is equal to the `length` argument. 

### Syntax
  ```js
  string_fill_zero(string, size, [on_left=true]);
  ```

| Argument | Type | Description |
| :--- | :---: | :--- |
| string | String | The string to fill |
| size | Int | The final size of the string |
| on_left | Bool | If the string will be filled on the left side. (default = true) |
### Returns
  ```js
  String
  ```

### Example
```js
var _str = "123";
var _size = 9;
var _score_str = string_fill_zero(_str, _size);

show_debug_message(_str_filled);
```

The above code will set the var `_str_filled` as an string filled with 0's on the left side and the show on console. The result will be `0000000123`.

---

# string_split
Returns an array from a string divided on substrings by a separator.

### Syntax
  ```js
  string_split(string, separator);
  ```

| Argument | Type | Description |
| :--- | :---: | :--- |
| string | String | The string to strip |
| separator | String | The separator to divide the string |
### Returns
  ```js
  Array
  ```

### Example
```js
var _str = "Hello, World!";
var _sep = ", ";
var _str_arr = string_split(_str, _sep);

show_debug_message(_str_arr);
```

The above code will set the var `_str_arr` as an array with the string divided on substrings and the show on console. The result will be `["Hello", "World!"]`.

---

# string_contains
Returns true if the string contains the substring.

### Syntax
  ```js
  string_contains(string, substring);
  ```

| Argument | Type | Description |
| :--- | :---: | :--- |
| string | String | The string to check |
| substring | String | The substring to use |
### Returns
  ```js
  Bool
  ```

### Example
```js
var _str = "Hello, World!";
var _sub = "World";

if (string_contains(_str, _sub)) {
    show_debug_message("World found!");
}
```

The above code will show on console the message `World Found!` since the string contains the substring.

---

<div style="display: flex; justify-content: space-between; align-items: center;">
  <div style="text-align: left; width: 50%">
    <h3>
      Prev: 
      <a href="Sprites.md">Sprites</a>
    </h3>
  </div>

  <div style="text-align: right; width: 50%">
    <h3>
      Next: 
      <a href="Structs.md">Structs</a>
    </h3>
  </div>
</div>