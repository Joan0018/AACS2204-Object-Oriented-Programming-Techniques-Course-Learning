# Java String equals()

### Usage
The `equals()` method returns `true` if two strings are identical and `false` if the strings are different.

### Example

```sh
class Main {
  public static void main(String[] args) {
    String str1 = "Learn Java";
    String str2 = "Learn Java";

    // comparing str1 with str2
    boolean result = str1.equals(str2);

    System.out.println(result);
  }
}
```
#### Output
>Output: true

### Syntax of equals()
The syntax of string `equals()` method is:
```sh
string.equals(String str)
```

### equals() Arguments
The `equals()` method takes a single argument.
- **str** - the string to be compared

### equals() Return Value
- **returns true** if the strings are equal
- **returns false** if the strings are not equal
- **returns false** if the `str` argument is `null`


### Example: Java String equals()
```sh
class Main {
  public static void main(String[] args) {
    String str1 = "Learn Java";
    String str2 = "Learn Java";
    String str3 = "Learn Kolin";
    boolean result;

    // comparing str1 with str2
    result = str1.equals(str2);
    System.out.println(result);  // true

    // comparing str1 with str3
    result = str1.equals(str3);

    System.out.println(result);  // false

    // comparing str3 with str1
    result = str3.equals(str1);
    System.out.println(result);  // false
  }
}
```
Here,
- `str1` and `str2` are equal. Hence, `str1.equals(str2)` returns `true`.
- `str1` and `str3` are not equal. Hence, `str1.equals(str3)` and `str3.equals(str1)` returns `false`.

### Example:  Check if Two Strings are Equal
```sh
class Main {
  public static void main(String[] args) {
    String str1 = "Learn Python";
    String str2 = "Learn Java";

    // if str1 and str2 are equal, the result is true
    if (str1.equals(str2)) {

      System.out.println("str1 and str2 are equal");
    }
    else {
      System.out.println("str1 and str2 are not equal");
    }
  }
}
```
#### Output
>str1 and str2 are not equal

### Example: Case-Sensitive Comparison
The `equals()` method performs case-sensitive comparison. Meaning `"Java"` and `"java"` are considered different strings.

```sh
class Main {
  public static void main(String[] args) {
    String str1 = "Java";
    String str2 = "java";
    Boolean result;

    // comparing str1 with str2
    result = str1.equals(str2);

    System.out.println(result);  // false
  }
}
```
