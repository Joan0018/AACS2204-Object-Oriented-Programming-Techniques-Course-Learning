# Java Character isDigit() Method

### Usage
The `isDigit()` function returns `true` if a character sent as a parameter is `digit`; otherwise, it returns `false`.

![image](https://github.com/Joan0018/AACS2204-Object-Oriented-Programming-Techniques-Course-Learning/assets/66239936/3118101e-69a6-45fb-ab60-e5f20b5022f7)


### Syntax of isDigit()
The syntax of character `isDigit()` method is:
```sh
public static boolean isDigit(char character) 
```

### isDigit() Parameters
- **ch** - It is the character that needs to be tested.

### isDigit() Return Value
This method returns a boolean value true if the character is a digit, otherwise false.

### Example 1

```sh
public class CharacterDemo {
   public static void main(String[] args) {

      // create 2 char primitives ch1, ch2
      char ch1, ch2;

      // assign values to ch1, ch2
      ch1 = '9';
      ch2 = 'V';

      // create 2 boolean primitives b1, b2
      boolean b1, b2;

      // assign isDigit results of ch1, ch2 to b1, b2
      b1 = Character.isDigit(ch1);
      b2 = Character.isDigit(ch2);
      String str1 = ch1 + " is a digit is " + b1;
      String str2 = ch2 + " is a digit is " + b2;

      // print b1, b2 values
      System.out.println( str1 );
      System.out.println( str2 );
   }
}
```
#### Output
```sh
9 is a digit is true
V is a digit is false
```
