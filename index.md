# Looking Closer At Wellesley's 7:1 Student to Faculty Ratio

_@author Annabel U (auhlman@wellesley.edu)_ <br>
Over the month of January, I've been exploring different datasets related to Wellesley, specifically the accessibility and availability of different courses and disciplines from a historic perspective. This was part of the Wellesley Data Collective, which you can check out [here](https://wellesleydatacollective.wordpress.com/)!

## Class Size and Student to Faculty Ratio by Discipline

There are so many factors to consider when picking a college, and one of the biggest is size. Large schools often tout access to resources while small schools often advertise close relationships with faculty, usually through a low student to faculty ratio. Wellesley claims a 7:1 student to faculty ratio, with a average class size of 17 students, according to the [Office of Instutional Research](https://www.wellesley.edu/oir/facts#:~:text=About%20Academics,is%2017%20students%20per%20class.). <br>
As Wellesley students, we know that the size of class you're in often depends on the department of the class - STEM classes seem to be larger and usually packed to the point that students are turned down or have to apply for a spot. <br>
With these themes in mind, I sought to look at the **average class size** and **student to faculty ratio** not for the whole school, but **by discipline.**

### 1. Average Class Size by Discipline
To calculate the average class size, I used excel sheets of all courses offered each semester from 2000-2020. These gave the CRN, Course, Title, Meeting Location, Times, and all other information that would be available for a class on the course browser. For each semester and department, I extracted the number of classes offered (assuming one professor per class), and number of students enrolled in the classes. I then calculated a simple ratio of number of students to number of professors, aka the average class size for that department for the selected semester. 
This produced a plot looking like: <br>
![Image](https://user-images.githubusercontent.com/77770436/106404047-72321200-63d5-11eb-952a-50e1ec0231a2.png)
<br>
The graph itself looks a bit crazy, but with class offerings varying each semester, the datapoints do jump around quite a bit. Humanities classes definitely have the lowest average class size over the whole twenty-year period, while the natural sciences seem to overtake the social sciences around 2013. 
<br>
<br>

### 2. Student to Faculty Ratio by Discipline
The average class size is a bit different than the student to faculty ratio, however. To calculate this, I collected the ***number of students enrolled*** in a department of a a certain discipline, divided by the number of faculty members in that department. I gathered fall enrollment data from the OIR's website, they have a bunch of interesting data accessible [here](https://www.wellesley.edu/oir/factbook/fall-enrollment-detail). <br>
This is what the raw data looked like after a bit of cleaning, with each column being a count of students in that major:
![Image](https://user-images.githubusercontent.com/77770436/106400765-9e916280-63c4-11eb-8cea-d179c6deed2e.PNG)<br>
It should be noted that I did not include all the students who are 'undeclared,' which was about half of the total students (think all first-years and sophomores). Resultingly, this is going to make the raio a lot smaller than it actually is.  <br>
<br> The ***number of faculty members*** I gathered from the [Faculty Roster](https://www.wellesley.edu/provost/facultyroster), using the [Wayback Machine](https://web.archive.org/web/2020*/https://www.wellesley.edu/provost/facultyroster) to access archived versions of the page. Using Selenium, I was able to scrape professor information back to 2013, when the earliest version of the page was saved. With (a lot) of cleaning, the final data showed this. <br>
![Image](https://user-images.githubusercontent.com/77770436/106404073-86760f00-63d5-11eb-8e6b-0d3fc0cd3cec.png)
<br>
Of course, all the ratios are lower than 7:1 since the vast number of undeclared students are not included. But we do notice that ***classes in the humanities have a significantly lower student to faculty ratio*** than the other two disciplines. Social sciences are just right above natural sciences, which seems to fluctuate a lot. <br>
The humanities departments also have the most consistent ratio across time, whereas the social sciences dipped in 2016, and the natural sciences changing almost every other year. <br>
<br>
### Looking Forward
These results are just the product of my curiosity and interest, and definitely have a lot of room for improvement. Because I was looking back over such a long period, there were changes in the ways that departments were named, or formatting of faculty info, or html code on the website. As a result, the data isn't perfect, so if you're interested, look into my code and data I used (linked below), or reach out to me! 
<br>
<br>
<br>
```markdown
### still interested?
Check out my code in my github repository [here](https://github.com/annabelu/wdc_jan21)
Learn more about the Wellesley Data Collective [here](https://wellesleydatacollective.wordpress.com/)
```
