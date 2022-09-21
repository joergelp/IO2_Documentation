# Teacher View

![Teacher View Diagram](../docs/img/teacherView/teacherViewUsageDiagram.png)

Once you have created the **external tool activity** ![](../docs/img/externalTool2.png) or ![](../docs/img/externalTool.png) and you have displayed it, you will see the welcome page:

![Get Started Page](../docs/img/teacherView/getStartedPage.png)

Simply, click on **Get Started** button

Teacher Control Center appears:
![Teacher Control Center](../docs/img/teacherView/teacherViewControlCenter.png)

At the beginning, every counter is **0**:
- exercises
- usage
- grades 

## Creating an exercise

As JuezLTI uses [_YAPExIL_](https://raw.githubusercontent.com/FGPE-Erasmus/format-specifications/master/schemas/yapexil.schema.json) format to store all exercise types, the interface to create exercises is the same for programming, databases or markup languages exercises.

Image below shows the form to define exercises:
![Create Exercise Form](../docs/img/teacherView/teacherViewCreateExerciseForm.png)

You can create a new Java exercise using next data:
- **Exercise Title**: `Welcome`
- **Keywords**: `Input, Output`
- **Exercise statement**: Write a Java program to print `Hello ` followed by a name received by standard input.

- **Code solution**: 
```
import java.util.Scanner;

public class Main {

    public static void main(String[] args)
    {
        Scanner input = new Scanner (System.in);
        String name = input.next();
        System.out.print("Hello "+name);
    }
}
```

- **With these inputs**: `Charles`

- **Expect these outputs**: `Hello Charles`

- **Add library**: _At the moment it is used only to provide a script with initial data to **test database exercises**_.

## Importing exercises from Authorkit
