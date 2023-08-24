# Java String toLowerCase()

### Usage
The `toLowerCase()` method converts all characters in the string to lowercase characters.

### Example

```sh
class Main {
  public static void main(String[] args) {
    String str1 = "JAVA PROGRAMMING";

    // convert to lower case letters
    System.out.println(str1.toLowerCase());

  }
}
```
#### Output
>Output: java programming

### Syntax of toLowerCase()
The syntax of string `toLowerCase()` method is:
```sh
string.toLowerCase()
```
Here, `string` is an object of the `String` class.

### toLowerCase() Parameters
The `toLowerCase()` method does not take any parameters.

### toLowerCase() Return Value
- returns a string with all upper case letters converted to lowercase letters


### Example: Java toLowerCase()
```sh
class Main {
  public static void main(String[] args) {
    String str1 = "Learn Java";
    String str2 = "Java123";

    // convert to lowercase letters
    System.out.println(str1.toLowerCase());  // "learn java"
    System.out.println(str2.toLowerCase());  // "java123"

  }
}
```
As you can see from the above example, `toLowerCase()` converts all uppercase letters to lower case letters.
