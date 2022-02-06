### DS-GA 1001 Final Project: Predicting DS Salaries based on qualitative factors.
### By Giulio Duregon, Joby George, Howell Lu, Jonah Poczobutt, Alexandre Vives

# Goals of the project

The main goals of this project are to:

    1. Data Exploration and understanding
    2. Statistical analysis of the Dataset 
    3. Predict Data Science salaries
    

## Background on Data

The dataset we are using for this project can be found on [kaggle](https://www.kaggle.com/jackogozaly/data-science-and-stem-salaries). The data was scraped from levels.fyi and had some cleaning done to it before being uploaded onto kaggle.

There are 62,000 rows and 29 columns, described below:
      1. Timestamp: Date the user account was created (and therefore the data was inputted)
      2. Company: Company name
      3. Level: Position level (it varies across companies)
      4. Title: Position title
      5. Totalyearlycompensation: Total yearly salary (includes bonus)
      6. Location: City where the job takes place
      7. Yearsofexperience: Total years of experience
      8. Yearsatcompany: Years the user has worked for the current company
      9. Tag: Additional title details
      10. Basesalary: Yearly salary without including bonus
      11. Stockgrantvalue: Value of the total stock in contract
      12. Bonus: Bonus obtained in the last year
      13. Gender: Gender of the user
      14. Otherdetails: Additional details of the job
      15. Cityid: ID of the city
      16. Dmaid: Value related to location
      17: DoctorateDegree: Binary variable whether the user had a Doctorate Degree
      18. Master's Degree: Binary variable whether the user had a Master's Degree
      19. Bachelor's Degree: Binary variable whether the user had a Bachelor's Degree
      20. Highschool Degree: Binary variable whether the user had a Highschool Degree
      21. Race_Asian: Binary variable whether the user is asian
      22. Race_White: Binary variable whether the user is white
      23. Race_Black: Binary variable whether the user is black
      24. Race_Hispanic: Binary variable whether the user is hispanic
      

## Motivating Factor for this Project

As Data Science graduate students at New York University's Center for Data Science, the team was naturally intrigued to learn what factors are most important with salaries of Data Science and STEM employees. 


## Helpful tips on collaborative working

The code below was used to read a csv file directly from GitHub:
    url = 'https://raw.githubusercontent.com/jgeorge313/DS_GA_1001_Capstone/main/Levels_Fyi_Salary_Data.csv'
    data = pd.read_csv(url)
    
The code bellow was used to run github scripts remotely in Jupyter notebook
    !curl -Os <raw_github_script_url>
    %run <script_name.ipynb>