# Ex05-Rec-JaggedArray
## Aim:
To write a C# program to create a sample CPU usage on a network with 4 nodes using a jagged array.
## Algorithm:
### Step1:
Start.

### Step2:
Declare a Jagged Array for four element.

### Step3:
Initialize the elements.

### Step4:
Accessing the elements.

### Step5:
Stop.

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
        for(int i=0; i<4; i++)
        {
            for(int j=0; j<array[i].Length; j++)
            {
                array[i][j] = i*j+70;
            }
        }
        for(int i=0; i<array.Length; i++)
        {
            for(int j=0;j<array[i].Length; j++)
            {
                Console.WriteLine("CPU usage at node"+ i +" is "+ array[i][j]+"%");
            }
            Console.WriteLine();
        }
    }
}
```

## Output:
![Online C# Compiler - online editor - Google Chrome 07-05-2022 11_06_24](https://user-images.githubusercontent.com/75235386/167240177-e9003e35-d4b2-4bcf-84b7-2d9ee6011e1f.png)

## Result:
Thus, the C# program to create a sample CPU usage on a network with 4 nodes using a jagged array is executed successfully.
