# Java String toCharArray()

### Usage
It converts a `String` object into an array of characters (`char[]`).

### Example

```sh
public class Main {
    public static void main(String[] args) {
        String str = "Hello";
        char[] charArray = str.toCharArray();
        
        // Print each character
        for (char c : charArray) {
            System.out.println(c);
        }
    }
}
```

#### Output
```sh
H
e
l
l
o
```

### Syntax of toCharArray()
The syntax of string `toCharArray()` method is:
```sh
string.toCharArray()
```
Here, `string` is an object of the `String` class.
