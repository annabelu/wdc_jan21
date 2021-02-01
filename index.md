# Looking Closer At Wellesley's 7:1 Student to Faculty Ratio

_@author Annabel U (auhlman@wellesley.edu)_ <br>
Over the month of January, I've been exploring different datasets related to Wellesley, specifically the accessibility and availability of different courses and disciplines from a historic perspective. This was part of the Wellesley Data Collective, which you can check out [here](https://wellesleydatacollective.wordpress.com/)!

## Class Size and Student to Faculty Ratio by Discipline

There are so many factors to consider when picking a college, and one of the biggest is size. Large schools often tout access to resources while small schools often advertise close relationships with faculty, usually through a low student to faculty ratio. Wellesley claims a 7:1 student to faculty ratio, with a average class size of 17 students, according to the [Office of Instutional Research](https://www.wellesley.edu/oir/facts#:~:text=About%20Academics,is%2017%20students%20per%20class.). <br>
As Wellesley students, we know that the size of class you're in often depends on the department of the class - STEM classes seem to be larger and usually packed to the point that students are turned down or have to apply for a spot. <br>
With these themes in mind, I sought to look at the **average class size** and **student to faculty ratio** not for the whole school, but **by discipline.**

### 1. Average Class Size by Discipline
To calculate the average class size, I used excel sheets of all courses offered each semester from 2000-2020. These gave the CRN, Course, Title, Meeting Location, Times, and all other information that would be available for a class on the course browser. For each semester and department, I extracted the number of classes offered (assuming one professor per class), and number of students enrolled in the classes. I then calculated a simple ratio of number of students to number of professors, aka the average class size for that department for the selected semester. 
This produced a plot looking like:
![Image](https://user-images.githubusercontent.com/77770436/106404047-72321200-63d5-11eb-952a-50e1ec0231a2.png)

### 2. Student to Faculty Ratio by Discipline
The average class size is a bit different than the student to faculty ratio, however. To calculate this, I collected the ***number of students enrolled*** in a department of a a certain discipline, divided by the number of faculty members in that department. I gathered fall enrollment data from the OIR's website, they have a bunch of interesting data accessible [here](https://www.wellesley.edu/oir/factbook/fall-enrollment-detail). <br>
This is what the raw data looked like after a bit of cleaning, with each column being a count of students in that major:
![Image](https://user-images.githubusercontent.com/77770436/106400765-9e916280-63c4-11eb-8cea-d179c6deed2e.PNG)<br>
It should be noted that I did not include all the students who are 'undeclared,' which was about half of the total students (think all first-years and sophomores). Resultingly, this is going to make the raio a lot smaller than it actually is.  <br>
<br> The ***number of faculty members*** I gathered from the [Faculty Roster](https://www.wellesley.edu/provost/facultyroster), using the [Wayback Machine](https://web.archive.org/web/2020*/https://www.wellesley.edu/provost/facultyroster) to access archived versions of the page. Using Selenium, I was able to scrape professor information back to 2013, when the earliest version of the page was saved. With (a lot) of cleaning, the final data showed this. <br>
![Image](https://user-images.githubusercontent.com/77770436/106404073-86760f00-63d5-11eb-8e6b-0d3fc0cd3cec.png)
<br>
It's interesting to see that 

```markdown
### still interested?
Check out my code in my github repository [here](https://github.com/annabelu/wdc_jan21)
Learn more about the Wellesley Data Collective [here](https://wellesleydatacollective.wordpress.com/)
```

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

