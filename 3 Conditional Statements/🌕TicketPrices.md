# Ticket Prices Problem
Write a C program that takes the age of a person as input and prints the ticket price according to the following criteria:

Children (age 0-12): 5 pesos
Teenagers (age 13-17): 8 pesos
Adults (age 18-59): 12 pesos
Seniors (age 60 and above): 6 pesos
Additionally, if a person is a student (age 18-59), they get a 20% discount on the ticket price.

<details>
<summary>Explanation</summary>
<br>
</details>


<details>
<summary>Answer</summary>
<br>

``` c
int main() {
    int age;
    char isStudent;

    // Input the person's age
    printf("Enter the person's age: ");
    scanf("%d", &age);

    // Input whether the person is a student (y/n)
    printf("Is the person a student? (y/n): ");
    scanf(" %c", &isStudent);

    // Determine and display the ticket price
    if (age >= 0 && age <= 12) {
        printf("Ticket Price: 5 pesos\n");
    } else if (age >= 13 && age <= 17) {
        printf("Ticket Price: 8 pesos\n");
    } else if (age >= 18 && age <= 59) {
        if (isStudent == 'y' || isStudent == 'Y') {
            printf("Ticket Price: %.2f  pesos\n", 0.8 * 12.0);
        } else {
            printf("Ticket Price: 12 pesos\n");
        }
    } else if (age >= 60) {
        printf("Ticket Price: 6 pesos\n");
    } else {
        printf("Invalid age.\n");
    }

    return 0;
}
```
</details>