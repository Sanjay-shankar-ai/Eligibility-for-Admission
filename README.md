# Eligibility-for-Admission

## Aim:
To write C# program to find the eligibility for admission to an engineering course

## Algorithnm:
### Step 1:
Create a new class called Admission.

### Step 2:
Create variables of respective data types to store marks and name.

### Step 3:
Calculate the total and store it.

### Step 4:
The conditions for admission are:
Marks in maths >= 65 & Marks in physics >=55 & Marks in chemistry >=50 & Total marks in all three subjects >= 180 or total in maths and physics >= 140

### Step 5:
Use Nested if to check whether someone is eligible for admission or not.

### Step 6:
Print the status of the program.

### Step 7:
End of program.

## Program:
```
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace LabExp1
{
    class Admission
    {
        static void Main(string[] args)
        {
            int mat, phy, chem;
            int tot, map;
            string name;
            Console.Write("Enter a Name:");
            name = Console.ReadLine();
            Console.Write("Enter marks in maths:");
            mat = Convert.ToInt32(Console.ReadLine());
            Console.Write("Enter marks in physics:");
            phy = Convert.ToInt32(Console.ReadLine());
            Console.Write("Enter marks in chemistry:");
            chem = Convert.ToInt32(Console.ReadLine());
            tot = mat + phy + chem;
            map = mat + phy;
            if(mat>=65 && phy>=55 && chem >= 50)
            {
                if(tot>=180 || map >= 140)
                {
                    Console.WriteLine(name+" eligible for admission");
                }
                else
                {
                    Console.WriteLine(name+" Not eligible for admission");
                }
            }
            else
            {
                Console.WriteLine(name+" Not eligible for admission");
            }
        }
    }
}
```


## Output:
![2023-03-17 (1)](https://user-images.githubusercontent.com/94231938/225823452-f1289284-b2e4-4104-9b57-7770c2af58d4.png)



## Result:
A C# program is written to find the eligibility for admission to an engineering course and has been successfully executed.
