## EX NO:5
## DATE:11.5.22
# <p align="center">JaggedArray
## Aim:
To write a C# program to create a sample CPU usage on a network with 4 nodes using a jagged array.
## Algorithm:
### Step1:
Start
### Step2:
Create a jagged array of 4arrays.
```
int[][] array = new int[4][];
```
### Step3:
Give the sample CPU usage in the jagged array. 
### Step4:
Print the sample CPU usage in the jagged array. 
### Step5:
stop


## Program:
```c#
using System;

class CPUactivity

{

    public static void Main(String[] args)

    {

        int[][] array = new int[4][];

        array[0] = new int[3];

        array[1] = new int[5];

        array[2] = new int[6];

        array[3] = new int[4];

        for (int i = 0; i < 4; i++)

        {

            for (int j = 0; j < array[i].Length; j++)

            {
                array[i][j] = i * j + 70;

            }

        }
        for (int i = 0; i < array.Length; i++)

        {

            for (int j = 0; j < array[i].Length; j++)

            {

                Console.WriteLine("CPU usage at node"+ i + " is "+ array[i][j]+" % ");

            }

            Console.WriteLine();

        }
    }
}
```

## Output:
![Screenshot (303)](https://user-images.githubusercontent.com/75235090/167241014-da1bda93-2042-4ff4-a442-15c0163d6242.png)

## Result:
Thus,C# program to create a sample CPU usage on a network with 4 nodes using a jagged array is executed successfully.
