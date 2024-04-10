# Java-Guess-a-number
User inputs a number until guesses the correct one

```java
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {

      int guess = 32;

      Scanner scanner = new Scanner(System.in);    
      System.out.println("Guess a number: ");

      int userGuess = scanner.nextInt();

      while (userGuess != guess) {
        if (userGuess < guess) { 
          System.out.println("Enter a bigger number!");
        } else if (userGuess > guess){
          System.out.println("Enter a smaller number!");
        } 

        userGuess = scanner.nextInt();

        }
        System.out.println("You have guessed it! The right number is " + guess);
    }
}
scanner.close();
}
}
```
