# Java String trim()

### Usage
The `trim()` method removes any leading (starting) and trailing (ending) whitespaces from the specified string.

### Example

```sh
class Main {
  public static void main(String[] args) {
    String str1 = "   Learn Java Programming      ";

    System.out.println(str1.trim());

  }
}
```
#### Output
>Output: Learn Java Programming

### Syntax of trim()
The syntax of string `trim()` method is:
```sh
string.trim()
```
Here, `string` is an object of the `String` class.

### trim() Parameters
- the `trim()` method doesn't take any parameters

### trim() Return Value
- returns a string with leading and trailing whitespace removed
- returns the original string if there is no whitespace in the start or the end of the string

#### Note:
In programming, whitespace is any character or series of characters that represent horizontal or vertical space. For example: space, newline `\n`, tab `\t`, vertical tab `\v` etc.


### Example: Java String trim()
```sh
class Main {
  public static void main(String[] args) {
    String str1 = "     Learn   Java Programming ";
    String str2 = "Learn\nJava Programming\n\n   ";

    System.out.println(str1.trim()); // Learn   Java Programming
    System.out.println(str2.trim()); 
    //Learn
    //Java Programming
  }
}
```

Here, `str1.trim()` returns
```sh
"Learn   Java Programming"
```
Similarly, `str2.trim()` returns
```sh
"Learn\nJava Programming"
```
As you can see from the above example, the `trim()` method only removes the leading and trailing whitespace. It doesn't remove whitespace that appears in the middle.

### Remove All Whitespace Characters
If you need to **remove all whitespace characters from a string**, you can use the _String replaceAll() method_ with proper regex.

```sh
class Main {
  public static void main(String[] args) {
    String str1 = "Learn\nJava \n\n   ";
    String result;

    // replace all whitespace characters with empty string
    result = str1.replaceAll("\\s", "");

    System.out.println(result);   // LearnJava
  }
}
```
