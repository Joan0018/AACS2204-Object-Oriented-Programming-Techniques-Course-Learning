# Java String replace()

### Usage
The `replace()` method replaces each matching occurrence of a character/text in the string with the new character/text.

### Example
```sh
class Main {
  public static void main(String[] args) {
    String str1 = "bat ball";

    // replace b with c
    System.out.println(str1.replace('b', 'c'));

  }
}

// Output: cat call
```

### Syntax of replace()
The syntax of the `replace()` method is either
```sh
string.replace(char oldChar, char newChar)
```
or
```sh
string.replace(CharSequence oldText, CharSequence newText)
```
Here, `string` is an object of the `String` class.

### replace() Parameters
To replace a single character, the `replace()` method takes these two parameters:
- **oldChar** - the character to be replaced in the string
- **newChar** - matching characters are replaced with this character

To replace a substring, the `replace()` method takes these two parameters:
- **oldText** - the substring to be replaced in the string
- **newText** - matching substrings are replaced with this string

### replace() Return Value
- The `replace()` method returns a new string where each occurrence of the matching character/text is replaced with the new character/text.

### Example 1: Java String replace() Characters
```sh
class Main {
  public static void main(String[] args) {
    String str1 = "abc cba";

    // all occurrences of 'a' is replaced with 'z'
    System.out.println(str1.replace('a', 'z'));  // zbc cbz

    // all occurences of 'L' is replaced with 'J'
    System.out.println("Lava".replace('L', 'J'));  // Java

    // character not in the string
    System.out.println("Hello".replace('4', 'J'));  // Hello

  }
}
```
#### Note
```sh
If the character to be replaced is not in the string, replace() returns the original string.
```

### Example 2: Java String replace() Substrings
```sh
class Main {
  public static void main(String[] args) {
    String str1 = "C++ Programming";

    // all occurrences of "C++" is replaced with "Java"
    System.out.println(str1.replace("C++", "Java"));  // Java Programming


    // all occurences of "aa" is replaced with "zz"
    System.out.println("aa bb aa zz".replace("aa", "zz")); // zz bb zz zz

    // substring not in the string
    System.out.println("Java".replace("C++", "C")); // Java
  }
}
```
#### Note
```sh
If the substring to be replaced is not in the string, replace() returns the original string.
```

It is important to note that the `replace()` method replaces substrings starting from the start to the end. For example,
```sh
"zzz".replace("zz", "x") // xz
```

The output of the above code is `xz`, not `zx`. It's because the `replace()` method replaced the first `zz` with `x`.

