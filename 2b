#include <stdio.h>
#include <string.h>

// Define a structure to represent a student
struct Student {
    char name[100];
    int rollNumber;
    int marks[3];
    int totalMarks;
    float averageMarks;
};

// Function prototypes
void readStudentDetails(struct Student* student);
void calculateTotalAndAverageMarks(struct Student* student);
void displayStudentDetails(const struct Student* student);
struct Student findStudentWithHighestMarks(struct Student students[], int n);

int main() {
    int n;

    // Prompt the user to enter the number of students
    printf("Enter the number of students: ");
    scanf("%d", &n);

    // Declare an array to store the students
    struct Student students[n];

    // Read details for each student
    for (int i = 0; i < n; ++i) {
        printf("Enter details for student %d:\n", i + 1);
        readStudentDetails(&students[i]);
        calculateTotalAndAverageMarks(&students[i]);
    }

    // Display details of each student
    printf("\nStudent Details:\n");
    for (int i = 0; i < n; ++i) {
        printf("Student %d:\n", i + 1);
        displayStudentDetails(&students[i]);
        printf("\n");
}
