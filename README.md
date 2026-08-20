# heyai
<br>It is about java code!
# Prime Numbers Up to N – Java

## Description

This Java program finds and displays all **prime numbers up to a given number `n`**. It also counts and displays the total number of prime numbers found.

The program uses a separate method `p1()` to check whether a number is prime.

## Concepts Used

* Java
* Methods
* `for` loop
* Conditional statements
* Modulus operator `%`
* Boolean return values
* Prime number logic

## How It Works

1. The value of `n` is set to `50`.
2. The program checks every number from `2` to `n`.
3. The `p1()` method checks whether each number is prime.
4. If the number is prime, it is printed.
5. The program counts the total number of prime numbers.
6. Finally, it displays the total count.

## Code

--->java
public class j6 {

    static boolean p1(int v) {
        if (v < 2) {
            return false;
        }

        for (int i = 2; i * i <= v; i++) {
            if (v % i == 0) {
                return false;
            }
        }

        return true;
    }

    public static void main(String[] args) {
        int n = 50;
        int cnt = 0;

        System.out.println("Prime numbers up to " + n + ":");

        for (int i = 2; i <= n; i++) {
            if (p1(i)) {
                System.out.print(i + " ");
                cnt++;
            }
        }

        System.out.println();
        System.out.println("Total primes found: " + cnt);
    }
}


##  Output

-->text
Prime numbers up to 50:
2 3 5 7 11 13 17 19 23 29 31 37 41 43 47
Total primes found: 15


## Complexity

* **Time Complexity:** `O(n√n)`
* **Space Complexity:** `O(1)`

## Learning Outcome

This program helps understand how to:

* Create and call methods in Java
* Check whether a number is prime
* Use loops and conditions
* Count values satisfying a condition
* Print formatted output

## Author

**Chandrashekar R**

