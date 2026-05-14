# Introduction

- Maven -> Dependency manager -> Allows for easy export external libraries into the code -> to make more complex software.

    ```
    maven --version
    ```

- JUnit -> Unit testing framework -> Not included in Java by default -> Brought in through the dependency manager 'Maven'.

# 1. Beginner Code Challenges

## i. Even or odd

- If number -> even; function returns "true".
- If number -> odd; function returns "false".

- Input -> Always Integer. 

- My Attempt: 

    ```java
    package com.linkedin.javacodechallenges;

    import java.util.Scanner;

    public class App {
        public static boolean isEven(int n) {
            // todo: implement functionality

            if (n % 2 == 0) {
                return true;
            } else {
                return false;
            }
            // return false;
        }

        public static void main(String[] args) {
            Scanner scanner = new Scanner(System.in);

            System.out.println("Enter a number: ");
            int userNum = scanner.nextInt();
            System.out.println("Is the number even? " + isEven(userNum));

            scanner.close();
        }
    }
    ````
- Lecturer's Attempt:

    ```java
    package com.linkedin.javacodechallenges;

    import java.util.Scanner;

    public class App {
        public static boolean isEven(int n) {
            // todo: implement functionality

            return n % 2 == 0;
        }

        public static void main(String[] args) {
            Scanner scanner = new Scanner(System.in);

            System.out.println("Enter a number: ");
            int userNum = scanner.nextInt();
            System.out.println("Is the number even? " + isEven(userNum));

            scanner.close();
        }
    }
    ```

- The Lecturer's attempt simplifies the entire function by getting rid of the 'if-else' statements and directly using the condition with the 'return' keyword, because `n % 2 == 0` will return 'true' or 'false' depending on the fulfillment of the condition.
