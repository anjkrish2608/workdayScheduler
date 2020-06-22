# Workday Scheduler


The website application was created by manipulating the CSS styling and HTML provided by Trilogy Education Services. The application allows the user to plan their work day and save their activities to their local storage by using the corresponding save buttons. The table structure of the HTML was created using JavaScript DOM manipulation. Through the use of **localStorage.getItem()** and **localStorage.setItem()** I was able to store the users initial input in the local storage when the button is clicked. 
Furthermore I learnt how to access the current time, as shown in the code quoted below: 
```
//setting colors
    var d = new Date();
    var currentHour= console.log(d.getHours());
    
```
This was learnt from [W3Schools.com](https://www.w3schools.com/JSREF/jsref_gethours.asp), as well as the similar functions used to construct the date in the header. Furthermore to create the date in the header with a *Ordinal Suffix* the following code was used:
```
//#Source https://bit.ly/2neWfJ2 
    const toOrdinalSuffix = num => {
      const int = parseInt(num),
        digits = [int % 10, int % 100],
        ordinals = ['st', 'nd', 'rd', 'th'],
        oPattern = [1, 2, 3, 4],
        tPattern = [11, 12, 13, 14, 15, 16, 17, 18, 19];
      return oPattern.includes(digits[0]) && !tPattern.includes(digits[1])
        ? int + ordinals[digits[0] - 1]
        : int + ordinals[3];
    };

```
I found this code at [w3resource.com](https://www.w3resource.com/javascript-exercises/fundamental/javascript-fundamental-exercise-122.php), the JavaScript in particular is referenced to a GitHub Repo called [30-seconds](https://github.com/30-seconds/30-seconds-of-code).
I enjoyed completing the backend JavaScript necessary to store the data. It was a long nit picking process but I am very proud of the final result shown below.

![day planner](./Develop/preview.png)

The functioning website can be found at [Work Day Scheduler](https://anjkrish2608.github.io/workdayScheduler/Develop/index.html).
## Challenges faced

Throughout the creation of this website I faced many challenges. The biggest and still present challenge I faced was the linking to and ensuring functioning of the premade CSS. The error occured when I introduced the ``` <form> ``` tag into the HTML which was necessary to ensure the function of the input field. Due to time management this was unable to be fixed. The CSS of the final result still needs some work and this is an area I am keen to improve on.

## Credits

Throughout creating this website to ensure correct syntax and resolve any errors [W3Schools.com](https://www.w3schools.com/) was consulted.

© 2019 Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.