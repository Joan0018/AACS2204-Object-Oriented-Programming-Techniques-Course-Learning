# Java String length()

### Usage
The `length()` method returns the number of characters in a string.

### Example
```sh
class Main {
  public static void main(String[] args) {
      String str1 = "Java is fun";

    // returns the length of str1
    int length = str1.length();


    System.out.println(str1.length());
  }
}
```

#### Output
> 11
> 
### Syntax of length()
The syntax of the string's `length()` method is:
```sh
string.length()
```

### length() Arguments
Ths `length()` method doesn't take any arguments.

### length() Return Value
- The `length()` method returns the length of a given string.

The length is equal to the number of characters (code units) in the string.

### Example: Java String length()
```sh
class Main {
    public static void main(String[] args) {
        String str1 = "Java";
        String str2 = "";

        System.out.println(str1.length());  // 4
        System.out.println("Java".length());  // 4

        // length of empty string
        System.out.println(str2.length());  // 0

       // new line is considered a single character
        System.out.println("Java\n".length()); // 5

        System.out.println("Learn Java".length()); // 10
    }
}
```
