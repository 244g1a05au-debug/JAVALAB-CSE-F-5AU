# Experiment3
## TITLE:3a.)implement constructor overloading in java
```
class Student {

	String name;
	int age;
	double marks;

	Student() {

	}

	Student(String name, int age, double marks) {

		this.name=name;
		this.age=age;
		this.marks=marks;

	}

	void display() {

		System.out.println("Name: "+name);
		System.out.println("Age: "+age);
		System.out.println("marks: "+marks);

	}

}
class Main {

	public static void main(String args[]) {

		Student std = new Student();
		std.display();

		Student std1 = new Student("Hari", 40, 67.8);
		std1.display();

	}
}
```
#output
<img width="134" height="120" alt="3a output" src="https://github.com/user-attachments/assets/c42cadd1-a1af-43ab-8e0a-76514fc3c35f" />
# experiment3b
## TITLE:3b.)class binary search
```
import java.util.Scanner;

class BinarySearch {

    int list[];
    int size;

    BinarySearch(int size) {
        list = new int[size];
        this.size = size;
    }

    void setList() {
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter the list items in Ascending Order.");

        for (int i = 0; i < size; i++) {
            System.out.print("Enter the value of " + (i + 1) + " item: ");
            list[i] = sc.nextInt();
        }
    }

    int binarySearch(int key) {

        int low = 0;
        int high = size - 1;

        while (low <= high) {
            int mid = (low + high) / 2;

            if (list[mid] == key)
                return mid;
            else if (list[mid] < key)
                low = mid + 1;
            else
                high = mid - 1;
        }
        return -1;
    }
}
```
# output
<img width="509" height="296" alt="Screenshot 2026-01-23 151836" src="https://github.com/user-attachments/assets/fd41b195-568f-4693-a462-8a2e2898aa41" />
# EXPERIMENT3c
## TITLE:3c.)binary search
```
import java.util.Scanner;

class Main {

    public static void main(String args[]) {

        Scanner sc = new Scanner(System.in);

        BinarySearch bs = new BinarySearch(10);
        bs.setList();

        System.out.print("Enter the key to search: ");
        int key = sc.nextInt();

        int index = bs.binarySearch(key);

        if (index == -1)
            System.out.println("Key item does not exist");
        else
            System.out.println("Key item exists at index: " + index);
    }
}
```
# output

<img width="225" height="64" alt="Screenshot 2026-01-23 152315" src="https://github.com/user-attachments/assets/14b8e18d-e2a1-471e-9053-edeb6a194138" />



