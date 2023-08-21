# Java String compareTo()

### Usage
The `compareTo()` method compares two strings lexicographically (in the dictionary order). The comparison is based on the Unicode value of each character in the strings.

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
#### Output
>Output: -1

### Syntax of compareTo()
The syntax of string `compareTo()` method is:
```sh
string.compareTo(String str)
```
Here, `string` is an object of the `String` class.

### compareTo() Parameters
Ths `compareTo()` method takes a single parameter.
- **str** - the string to be compared

### compareTo() Return Value
- **return 0** if the strings are equal
- **returns a negative integer** if the `string` comes before the `str` argument in the dictionary order
- **returns a positive integer** if the `string` comes after the `str` argument in the dictionary order


### Example: Java String compareTo()
```sh
class Main {
  public static void main(String[] args) {
    String str1 = "Learn Java";
    String str2 = "Learn Java";
    String str3 = "Learn Kolin";
    int result;

    // comparing str1 with str2
    result = str1.compareTo(str2);

    System.out.println(result);  // 0

    // comparing str1 with str3
    result = str1.compareTo(str3);

    System.out.println(result);  // -1

    // comparing str3 with str1
    result = str3.compareTo(str1);

    System.out.println(result);  // 1
  }
}
```
Here,
- `str1` and `str2` are equal. Hence, `str1.compareTo(str2)` returns 0.
- `str1` comes before `str3` in the dictionary order. Hence, `str1.compareTo(str3)` returns negative, and `str3.compareTo(str1)` returns positive.

### Example 2: Check if Two Strings are Equal
```sh
class Main {
  public static void main(String[] args) {
    String str1 = "Learn Python";
    String str2 = "Learn Java";
        
    // if str1 and str2 are equal, the result is 0
    if (str1.compareTo(str2) == 0) {

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

### Example 3: compareTo() With Case
The `compareTo()` method takes the letter case (uppercase and lowercase) into consideration.

```sh
class Main {
  public static void main(String[] args) {
    String str1 = "Learn Java";
    String str2 = "learn Java";
    int result;

    // comparing str1 with str2
    result = str1.compareTo(str2);

    System.out.println(result);  // -32
  }
}
```
When `"Learn Java"` is compared to `"learn Java"`, we do not get 0. It is because `compareTo()` takes the letter case into consideration.


The negative value indicates that the first differing character in `str1 (which is 'L')` has a lower ASCII value than the corresponding character in `str2 (which is 'l')`. The difference in ASCII values is 32.
