# Java String equalsIgnoreCase()

### Syntax of equalsIgnoreCase()
The syntax of the string `equalsIgnoreCase()` method is:
```sh
string.equalsIgnoreCase(String str)
```
Here, `string` is an object of the `String` class.

### equalsIgnoreCase() Parameters
Ths string `equalsIgnoreCase()` method takes a single parameter
- **str** - this string to be compared

### equalsToIgnoreCase() Return Value
- **returns true** if the strings are equal, ignoring case considerations
- **returns false** if the strings are not equal
- **returns false** if the `str` argument is `null`

### Example 1: Java String equalsIgnoreCase()
```sh
class Main {
    public static void main(String[] args) {
        String str1 = "Learn Java";
        String str2 = "learn java";
        String str3 = "Learn Kolin";
        Boolean result;

        // comparing str1 with str2
        result = str1.equalsIgnoreCase(str2);
        System.out.println(result); // true

        // comparing str1 with str3
        result = str1.equalsIgnoreCase(str3);
        System.out.println(result); // false

        // comparing str3 with str1
        result = str3.equalsIgnoreCase(str1);
        System.out.println(result); // false
    }
}
```
#### Output
> true
> false
> true

Here,
- `str1` and `str2` are equal if you do not consider case differences. Hence, `str1.equalsIgnoreCase(str2)` returns `true`.
- `str1` and `str3` are not equal. Hence, `str1.equalsIgnoreCase(str3)` and `str3.equalsIgnoreCase(str1)` returns `false`.

### Example 2: Check if Two Strings are Equal
```sh
class Main {
    public static void main(String[] args) {
        String str1 = "LEARN JAVA";
        String str2 = "Learn Java";
        
        // if str1 and str2 are equal (ignoring case differences),
        // the result is true
        if (str1.equalsIgnoreCase(str2)) {
            System.out.println("str1 and str2 are equal");
        }
        else {
            System.out.println("str1 and str2 are not equal");
        }
    }
}
```

#### Output
> str1 and str2 are equal
