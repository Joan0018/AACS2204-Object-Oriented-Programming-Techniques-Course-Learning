# Java String lastIndexOf()

### Syntax of lastIndexOf()
The syntax of string `lastIndexOf()` method is:
```sh
string.lastIndexOf(int ch, int index)
```
or
```sh
string.lastIndexOf(string str, int index)
```

### lastIndexOf() Parameters
To find the last index of a character, `lastIndexOf()` takes these two parameters:
- **ch** - the character whose last index is to be found
- **index** (optional) - if `index` is passed, the `ch` character is searched from start to this index

To find the last index of the specified substring within the string, `lastIndexOf()` takes these two parameters:
- **str** - the string whose last index is to be found
- **index** (optional) - if `index` is passed, the `str` string is searched from start to this index



### lastIndexOf() Return Value
- **returns the index** of the last occurrence of the specified character/string
- **returns -1** if the specified character/string is not found.


### Example: Java String lastIndexOf()
```sh
// Java String lastIndexOf() with only one parameter
class Main {
  public static void main(String[] args) {
    String str1 = "Learn Java";
    int result;

    // getting index of character 'J'
    result = str1.lastIndexOf('J');
    System.out.println(result); // 6

    // the last occurrence of 'a' is returned
    result = str1.lastIndexOf('a');
    System.out.println(result); // 9

    // character not in the string
    result = str1.lastIndexOf('j');
    System.out.println(result); // -1

    // getting the last occurrence of "ava"
    result = str1.lastIndexOf("ava");
    System.out.println(result); // 7

    // substring not in the string
    result = str1.lastIndexOf("java");
    System.out.println(result); // -1
  }
}
```
#### Note:
The character `'a'` occurs multiple times in the `"Learn Java"` string. The `lastIndexOf()` method returns the index of the last occurrence of `'a'` (which is 9).

### Example: lastIndexOf() With fromIndex Parameter
```sh
class Main {
  public static void main(String[] args) {
    String str1 = "Learn Java programming";
    int result;

    // search from index 0 to 4
    // searches the substring "Learn"
    result = str1.lastIndexOf('r', 4);
    System.out.println(result); // 3

    // search from index 0 to 12
    // searcheses the substring "Learn Java pr"
    result = str1.lastIndexOf('r', 12);
    System.out.println(result); // 12

    // string length is less than 100
    // searches the whole string
    result = str1.lastIndexOf('r', 70);
    System.out.println(result); // 15

    // searches the substring "Learn"
    result = str1.lastIndexOf("Java", 4);
    System.out.println(result); // -1
  }
}
```

#### Note:
- The last occurrence of `'r'` in the `"Learn Java programming"` string is at index 15. However, `str1.lastIndexOf('r', 4)` searches the substring `"Learn"`. The last index of `'r'` in `"Learn"` is at index 3.
- `str1.lastIndexOf('r', 12)` searches the substring `"Learn Java pr"`. The last index of `'r'` in `"Learn Java pr"` is at index 12.
- `str1.lastIndexOf("Java", 4)` searches the substring `"Learn"`. Since there is no `"Java"` in the `"Learn"` substring, the result is -1.
