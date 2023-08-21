# Java String replaceAll()

### Usage
The `replaceAll()` method replaces each substring that matches the regex of the string with the specified text.

### Example
```sh
class Main {
  public static void main(String[] args) {
    String str1 = "Java123is456fun";

    // regex for sequence of digits
    String regex = "\\d+";

    // replace all occurrences of numeric
    // digits by a space
    System.out.println(str1.replaceAll(regex, " "));


  }
}
```

#### Output
> Java is fun

### Syntax of replaceAll()
The syntax of the `replaceAll()` method is:
```sh
string.replaceAll(String regex, String replacement)
```
Here, `string` is an object of the `String` class.

### replaceAll() Parameters
The `replaceAll()` method takes two parameters.
- **regex** - a regex (can be a typical string) that is to be replaced
- **replacement** - matching substrings are replaced with this string

### replaceAll() Return Value
The `replaceAll()` method
- returns a new string where each occurrence of the matching substring is replaced with the **replacement** string.

### Example 1: Java String replaceAll()

```sh
class Main {
  public static void main(String[] args) {
    String str1 = "aabbaaac";
    String str2 = "Learn223Java55@";

    // regex for sequence of digits
    String regex = "\\d+";

    // all occurrences of "aa" is replaceAll with "zz"
    System.out.println(str1.replaceAll("aa", "zz"));  // zzbbzzac


    // replace a digit or sequence of digits with a whitespace
    System.out.println(str2.replaceAll(regex, " "));  // Learn Java @


  }
}
```
In the above example, `"\\d+"` is a regular expression that matches one or more digits. To learn more, visit Java regex.

### Escaping Characters in replaceAll()
The `replaceAll()` method can take a regex or a typical string as the first argument. It is because a typical string in itself is a regex.

In regex, there are characters that have special meaning. 
These metacharacters are:

```sh
\ ^ $ . | ? * + {} [] ()
```
If you need to match substring containing these metacharacters, you can either escape these characters using `\` or use the `replace()` method.

```sh
// Program to replace the + character
class Main {
  public static void main(String[] args) {
    String str1 = "+a-+b";

    // replace "+" with "#" using replaceAll()
    // need to escape "+"
    System.out.println(str1.replaceAll("\\+", "#"));  // #a-#b


    // replace "+" with "#" using replace()
    System.out.println(str1.replace("+", "#"));  // #a-#b

  }
}
```

As you can see, when we use the `replace()` method, we do not need to escape metacharacters.
