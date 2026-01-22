# EXPERIMENT 2C
## TITLE:2C.)java programe implement constructor
```
class Student {
String name;
int age;
int marks;
Student (String n, int a, int m) {
name = n;
age = a;
marks = m;
}
void display ( ) {
System.out.println ("Name: " + name);
System.out.println ("Age: " + age);
System.out.println ("Marks: " + marks);
}
public static void main(String[] args) {
Student S1 = new Student ("Alice", 20, 85);
S1.display ( );
}
}
```
# OUTPUT
![exp2c](https://github.com/user-attachments/assets/702ddee7-9aa9-4a46-af4d-9e5d5b3d817e)
