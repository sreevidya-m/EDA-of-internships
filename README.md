# Exploratory Data Analysis (EDA) Of Internships Data
<br>
Exploratory Data Analysis (EDA) is an approach to analyze the data so as to summarize its main characteristics, discover trends, patterns or anomalies in the data by using visualization techniques.
<br>The project involved performing EDA on the Internship Dataset. <br><br>
<b>Data Pre-Processing:</b><br><br>
For Data Preprocessing, the following steps were done:<br>
1. Checking and eliminating duplicate records <br>
2. Checking for wrong entries like symbols -,?,#,*,etc in the data <br>
3. Replacing 'Unknown' values in 'Stipend_per_month' column with NaN <br>
4. Finding missing values in each column <br>
5. Replacing the missing values in 'Skills Required' and 'Perks' column with 'None' and dropping the  missing values in 'Stipend_per_month' column <br>
6. Changing the datatype of 'Stipend_per_month' column to 'float64' <br>
7. Splitting the 'Perks' column into multiple columns like 'Certificate', 'LOR', 'Flexible_work_hrs', 'Job_Offer', 'Informal_Dress_Code','5_Days'and 'Free_Snacks' <br>
8. Making a new column 'No of Skills' by counting the number of skills in the 'Skills Required' Column. <br>
9. Changing 'Be an early applicant' in 'Applicants' column to '0 applicants' <br>
10. Extracting only the number in 'Applicants' column (eg: change from '33 applicants' to 33) <br>
11. Making a new column 'wfh' which has value '1' if the internship is of work from home type oe else '0' <br><br>
Thus, the dataset has been cleaned successfully and can now be used for analysis <br><br>
<b>Exploratory Data Analysis: </b><br><br>
The following analysis was done on the cleaned data:<br>
1. Finding the correlation between all numeric columns by using correlation matrix.
<br><i>Inference: It can be concluded that the Stipend per month and the number of applicants is not dependent on other attributes since the correlation with most attributes is negative and if any coorelation is positive, it is very low to be considered </i><br><br>
2. Analysis of Category wise Internships: number of internships, openings, stipend and applicants in each category
<br><i>Inferences: <br>
a. Maximum Internships are offered in the category 'Marketing' whereas Minimum Internships are offered in the category 'Humanities'<br>
b. Maximum number of openings are in Volunteering, Marketing and Computer Science whereas the least number of openings are in Architecture, Electronics and Humanities. <br>
c. Science Category Internships have the maxium average stipend whereas Volunteering category Internships have the minimum average stipend. <br>
d. Least no of applicants prefer doing 'Architecture' Internship whereas Internships like Mechanical, Finance, Volunteering, Content Writing, CS, HR, Marketing, Graphic Design and Commerce are higly popular among applicants and are preferred the most</i><br><br>
3. Analysis of No of skills required and the Stipend offered:
<br><i>Inference: Stipend per month for any internship is not determined by the number of skills required for the internship.<br></i><br>
4. Analysis of Internships with Certificate:
<br><i>Inferences: <br>
a. Maximum number of internships offered provide a certifcate <br>
b. The average stipend/month for internships without a certifcate is more than the internships with a certifiate. <br>
c. There is not much difference between the number of applications for both types of internships- with certificate and without certificate. <br></i><br>
5. Analysis of Internships with Job Offer:
<br><i>Inferences: <br>
a. Most number of internships floated do not have a potential job offer. <br>
b. Internships with a potential job offer gives higher avg stipend per month than Internships without Job offer <br>
c. Almost the same number of applicants prefer Internships with job offer and Internships without job offer. <br></i><br>
6. Analysis of Internships of Work From Home type:
<br><i>Inferences: <br>
a. Maximum Internships offered are of type 'Work from Home' <br>
b. 'Work from home' Internships gives lower avg stipend per month than other Internships<br>
c. 'Work from home' Internships are preferred more by applicants than other internships <br></i><br>
7. Analysis of Internships based on its Duration:
<br><i>Inferences: <br>
a. Maximum Internships offered are of duration 3 months whereas the least number of Internships offered are of duration 1.25 months and 24 months. <br>
b. Maximum Avg Stipend is offered in Internships of duration 12 months whereas the Minimum Avg Stipend is offered in Internships of duration 0.25 months
It can also be said that roughly the Avg Stipend increases as the duration of the Internship inreases.<br>
c. Maximum Applicants prefer Internships with duration of 1.5 months and very few Applicants prefer Internships with duration of 24 months and more <br></i><br>
8. Analysis of Location-wise Internships:
<br><i>Inferences: <br>
a. Maximum number of internships offered are 'Work from Home'
But considering only cities, Delhi, Bangalore, Mumbai and Pune have the maximum Internship opportunities. <br>
b. The Top 5 Internship locations in terms of average stipend/month is Bharatpur, Gurugaon, Jamnagar, Kottayam and Manipal
The Bottom 5 Internship locations in terms of average stipend/month is Bilbao, Dahanu, Haridwar, Pimpari and Bareilly.
This shows that average stipend also varies with Internship location.<br>
c. There is a huge requirement of interns for Work From Home type Internships. Delhi, Mumbai, Bangalore and Pune are among the top cities having huge requirements (on the basis of number of openings) <br></i><br>
9. Analysis of Stipends:
<br><i>Inferences: <br>
a. The density curve is right skewed which shows that the mean is greater than the median.
Maximum internships have stipend between Rs 0 and 10,000. There are very few internships with stipend more than Rs 20,000<br>
b. HoloSuit, Yamaha Motor Solution Pvt Ltd, Zeedup technologies and Dsigns Australia are among the top companies offering the highest stipend per month <br></i><br>
10. Analysis of Internships under Computer Science Category:
<br><i>Inferences: <br>
a. The highest requirement of interns (based on number of openings) in the Computer Science Category is for Web Development, Mobile App Development, Python Development, Front End Development and WordPress Development.<br>
b. Machine Learning, React Native and Mean Stack Development are among the the Highest Stipend Paying Titles in Computer Science category of Internships <br>
c. Web development, Python Development, Front End Development, Software Testing and Mobile App Development are among the most preferred job titles by applicants <br>
d. Some of the highest stipend paying companies in Computer science Category are Yamaha Motor Solution, Zeedup Technologies, Prachi Mishra, Yellow.ai and Findmycollege<br></i><br>
11. Analysis of Internships with Perks and Incentives:
<br><i>Inferences: <br>
a. 52.6% Internships provide 5 days a week <br>
b. 56.5% Internships provide Flexible Work Hours <br>
c. 70.9% Internships provide Letter of Recommendation <br>
d. Only 9.6% Internships provide Incentives <br>
e. 18.8% Internships allow Informal Dress Code <br>
f. 8.9% Internships provide Free Snacks and Bevarages<br></i><br>
