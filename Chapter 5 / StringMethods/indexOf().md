# Java String indexOf()

### Usage
The `indexOf()` method returns the index of the first occurrence of the specified character/substring within the string.

### Example

```sh
class Main {
  public static void main(String[] args) {
    String str1 = "Java is fun";
    int result;

    // getting index of character 's'
    result = str1.indexOf('s');

    System.out.println(result);
  }
}
```
#### Output
>Output: 6

### Syntax of indexOf()
The syntax of string `indexOf()` method is:
```sh
string.indexOf(int ch, int fromIndex)
```
or
```sh
string.indexOf(String str, int fromIndex)
```
Here, `string` is an object of the `String` class.

### indexOf() Parameters
To find the index of a character, `indexOf()` takes these two parameters:
- **ch** - the character whose starting index is to be found
- **fromIndex** (optional) - if `fromIndex` is passed, the `ch` character is searched starting from this index
To find the index of the specified substring within the string, `indexOf()` takes these two parameters:
- **str** - the string whose starting index is to be found
- **fromIndex** (optional) - if `fromIndex` is passed, the `str` string is searched starting from this index

### indexOf() Return Value
- **returns the index** of the first occurrence of the specified character/string
- **returns -1** if the specified character/string is not found.


### Example: Java String indexOf()
```sh
// Java String indexOf() with only one parameter
class Main {
  public static void main(String[] args) {
    String str1 = "Learn Java";
    int result;

    // getting index of character 'J'
    result = str1.indexOf('J');
    System.out.println(result); // 6

    // the first occurrence of 'a' is returned
    result = str1.indexOf('a');
    System.out.println(result); // 2

    // character not in the string
    result = str1.indexOf('j');
    System.out.println(result); // -1

    // getting the index of "ava"
    result = str1.indexOf("ava");

    System.out.println(result); // 7

    // substring not in the string
    result = str1.indexOf("java");

    System.out.println(result); // -1

    // index of empty string in the string
    result = str1.indexOf("");

    System.out.println(result); // 0
  }
}
```
#### Notes:
- The character `'a'` occurs multiple times in the `"Learn Java"` string. The `indexOf()` method returns the index of the first occurrence of `'a'` (which is 2).
- If the empty string is passed, `indexOf()` returns 0 (found at the first position. It is because the empty string is a subset of every substring.

### Example: indexOf() With fromIndex Parameter
```sh
  class Main {
  public static void main(String[] args) {
    String str1 = "Learn Java programming";
    int result;

    // getting the index of character 'a'
    // search starts at index 4
    result = str1.indexOf('a', 4);

    System.out.println(result);  // 7

    // getting the index of "Java"
    // search starts at index 8
    result = str1.indexOf("Java", 8);

    System.out.println(result);  // -1
  }
}
```

#### Notes:
- The first occurrence of `'a'` in the `"Learn Java programming"` string is at index 2. However, the index of second `'a'` is returned when `str1.indexOf('a', 4)` is used. It is because the search starts at index 4.
- The `"Java"` string is in the `"Learn Java programming"` string. However, `str1.indexOf("Java", 8)` returns -1 (string not found). It is because the search starts at index 8 and there is no `"Java"` in `"va programming"`.
