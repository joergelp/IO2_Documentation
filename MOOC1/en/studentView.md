# Student View

![Student View Diagram](../docs/img/studentView/studentViewUsageDiagram.png)

Once instructors have created the **external tool activity** ![](../docs/img/externalTool2.png) or ![](../docs/img/externalTool.png), students could see it in their course page:

![Select External Activity](../docs/img/studentView/selectingExternalActivity.png)

Student only need click on the External Activity. In this case, _Easy exercise_

A Student View similar to the image below appears:
![Student Form Page](../docs/img/studentView/studentViewFormPage.png)

On top of the page, the list of exercises that compose the activity is showed:

![Student View List Exercises](../docs/img/studentView/studentViewListExercises.png)

Example above shows an activity composed by three exercises, in one of the three possible states each:

- _orange_: the student didn't answer the exercise.
- _green_: the student solved the exercise.
- _red_: the student launched a wrong answer to the exercise.

Student can use the list of exercises to navigate thought the exercises, clicking on them.

After the list of exercises, the exercise's title and statement is found

![Student View Title and Statement](../docs/img/studentView/studentViewTitleStatement.png)

and the set of tests

![Student View Set of Tests](../docs/img/studentView/studentViewTests.png)

In those tests, student can view the output that corresponds each input. In the example above, if the code receives `Charles` it must return `Hello Charles`.

The student must code his solution on _Code Solution_ field, selecting previously in wich language will be coded the solution:

![Student View Answer](../docs/img/studentView/studentViewAnswer.png)

At bottom of the page the student will receive the grade and feedback of his answer.

Above, you can view the result of two different codes:

- Wrong answer:

```
import java.util.Scanner;

public class Main {

    public static void main(String[] args)
    {
        Scanner input = new Scanner (System.in);
        String name = input.next();
        System.out.print("Hello "+name+"!!");
    }
}
```
![Student View Wrong Answer](../docs/img/studentView/studentViewWrongAnswer.png)

- Right answer:

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
![Student View Right Answer](../docs/img/studentView/studentViewRightAnswer.png)

