# sql-challenge summary
**Data Engineering and Analysis**

In this assignment, my task was to perform data engineering and data analysis of employee data for my boss.
First,  with the help of QuickDBD app / an Entity Relationship (ER) Diagram was created for all 6 tables, where data types, primary keys, foreign keys, and other constraints were specified.

I utlized a pgAdmin, an open source administration and development platform, to build the database. Once the relationships were identified, I ran the queries in the pgAdmin and imported the CSV files into the corresponding SQL table. 

**Data Analysis**

For Data Analysis section, I used the pgAdmin to run the queries and the following tasks were performed:
- list details of each employee: employee number, last name, first name, sex, and salary.
- list first name, last name, and hire date for employees who were hired in 1986.
- list the manager of each department with the following information: department number, department name, the manager's employee number, last name, first name.
- list the department of each employee with the following information: employee number, last name, first name, and department name.
- list first name, last name, and sex for employees whose first name is "Hercules" and last names begin with "B."
- list all employees in the Sales department, including their employee number, last name, first name, and department name.
- list all employees in the Sales and Development departments, including their employee number, last name, first name, and department name.
- In descending order, list the frequency count of employee last names, i.e., how many employees share each last name.

**Bonus** - further analysis of employee salaries

Bonus (Optional)

My goal was to generate a visualization of the above data which I want to present to my boss:

1. In order to import the SQL database into Pandas: I used the started code given below:

        from sqlalchemy import create_engine
        engine = create_engine('postgresql://localhost:5432/<your_db_name>')
        connection = engine.connect()

By storing the password and username in the config, I was able to import the data into pandas.

2. In order to visualize the most common salary ranges for employees, a histogram was used. Most comon salary range is between $40,000 - $60,000; th min being $40,000 and max being $129,492.


3. Then, a bar chart of average salaries by title was created to visualize the salaries by professional titles. As you can see the technical leaders and the managers are highest paying positions.

As I examined the data, I was confident that the dataset was fake. So looked up my employee ID and found that my name was April Foolsday :). 
