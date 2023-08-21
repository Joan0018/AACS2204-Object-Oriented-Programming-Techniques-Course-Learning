# Java String compareTo()

### Usage
The `charAt()` method returns the character at the specified index.

### Example

```sh
class Main {
  public static void main(String[] args) {
    String str1 = "Learn Java";
    String str2 = "Learn Kolin";
    int result;

    // comparing str1 with str2
    result = str1.compareTo(str2);

    System.out.println(result);
  }
}
```
>Output: -1

### Syntax of charAt()
The syntax of string `charAt()` method is:
```sh
string.charAt(ing index)
```
Here, `string` is an object of the `String` class.

### charAt() Parameters
- **index** - the index of the character (an `int` value)

### charAt() Return Value
- returns the character at the specified `index`
  
`If the index passed to charAt() is negative or out of bounds, it throws an exception.`


### Example: Java String charAt()
```sh
class Main {
  public static void main(String[] args) {
    String str1 = "Learn Java";
    String str2 = "Learn\nJava";

    // first character
    System.out.println(str1.charAt(0));  // 'L'

    // seventh character
    System.out.println(str1.charAt(6));  // 'J'


    // sixth character
    System.out.println(str2.charAt(5));  // '\n'
  }
}
```

In Java, the index of Strings starts from **0**, not **1**. That's why `chartAt(0)` returns the first character. Similarly, `charAt(5)` and `charAt(6)` return the sixth and seventh character respectively.

### Note
If you need to find the index of the first occurrence of the specified character, use the _Java String indexOf()_ method.
