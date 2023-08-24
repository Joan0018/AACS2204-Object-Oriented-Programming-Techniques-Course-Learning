# Java Character isLetter() Method

### Usage
The `isLetter(char ch)` method of Character class determines whether the given(or specified) character is a letter or not.

### Syntax of isLetter()
The syntax of string `isLetter()` method is:
```sh
public static boolean isLetter(char ch)  
```

### isLetter() Parameters
- **ch** - It is the character that needs to be tested.

### isLetter() Return Value
The `isLetter(char ch)` method returns a `Boolean` value i.e. true if the given(or specified) character is a letter. Otherwise, the method returns false.

### Example 1

```sh
public class JavaCharacterisLetterExample1 {  
    public static void main(String[] args) {  
    // Create three char primitives ch1, ch2 and ch3.  
      char ch1, ch2, ch3;  
      // Assign the values to ch1, ch2 and ch3.  
      ch1 = 'A';  
      ch2 = '9';  
      ch3 = 'e';  
      // Create three boolean primitives b1, b2 and b3;  
      boolean b1, b2, b3;  
      // Check whether ch1, ch2 and ch3 are letters or not and assign the results to b1, b2 and b3.  
      b1 = Character.isLetter(ch1);  
      b2 = Character.isLetter(ch2);  
      b3 = Character.isLetter(ch3);  
  
      String str1 = "The character "+ch1 + " is a letter: " + b1;  
      String str2 = "The character "+ch2 + " is a letter: " + b2;  
      String str3 = "The character "+ch3 + " is a letter: " + b3;  
  
      // Print the values of b1, b2 and b3.  
      System.out.println( str1 );  
      System.out.println( str2 );  
       System.out.println( str3 );  
   }  
}  
```
#### Output
```sh
The character A is a letter: true
The character 9 is a letter: false
The character e is a letter: true
```

### Example 2
```sh
public class JavaCharacterisLetterExample2 {  
    public static void main(String[] args) {  
    // Create three char primitives ch1, ch2 and ch3.  
      char ch1, ch2, ch3;  
      // Assign the values to ch1, ch2 and ch3.  
      ch1 = '1';  
      ch2 = '*';  
      ch3 = 'e';  
      // Create three boolean primitives b1, b2 and b3;  
      boolean b1, b2, b3;  
      // Check whether if ch1, ch2 and ch3 are letters or not and assign the result to b1, b2 and b3.  
      b1 = Character.isLetter(ch1);  
      b2 = Character.isLetter(ch2);  
      b3 = Character.isLetter(ch3);  
  
      String str1 = "The character "+ch1 + " is a letter: " + b1;  
      String str2 = "The character "+ch2 + " is a letter: " + b2;  
      String str3 = "The character "+ch3 + " is a letter: " + b3;  
  
      // Print the values of b1, b2 and b3.  
      System.out.println( str1 );  
      System.out.println( str2 );  
       System.out.println( str3 );  
   }  
}  
```
#### Output
```sh
The character 1 is a letter: false
The character * is a letter: false
The character e is a letter: true
```

### Example 3
```sh
public class JavaCharacterisLetterExample3 {  
    public static void main(String[] args) {  
    // Create three char primitives ch1, ch2 and ch3.  
      char ch1, ch2, ch3;  
      // Assign the values to ch1, ch2 and ch3.  
      ch1 = '1';  
      ch2 = ')';  
      ch3 = '*';  
      // Create three boolean primitives b1, b2 and b3;  
      boolean b1, b2, b3;  
      // Check whether  ch1, ch2 and ch3 are letters or not and assign the result to b1, b2 and b3.  
      b1 = Character.isLetter(ch1);  
      b2 = Character.isLetter(ch2);  
      b3 = Character.isLetter(ch3);  
  
      String str1 = "The character "+ch1 + " is a letter: " + b1;  
      String str2 = "The character "+ch2 + " is a letter: " + b2;  
      String str3 = "The character "+ch3 + " is a letter: " + b3;  
  
      // Print the values of b1, b2 and b3.  
      System.out.println( str1 );  
      System.out.println( str2 );  
       System.out.println( str3 );  
   }  
}  
```

#### Output
```sh
The character 1 is a letter: false
The character ) is a letter: false
The character * is a letter: false
```
