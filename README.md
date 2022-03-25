# KurtNoe-Datahouse-Compatibility-Predictor
Code to take JSON files containing statistical scores of both a team and potential applicants. Takes these scores and uses them to calculate the compatibility of these applicants with the team to determine who is the best fit.

1. The application was created using the Python programming language and compiled using Jupyter Notebook. To access the code simply load the application file named 'KurtNoe_Datahouse_Compatibilty_Predictor' using Jupyter notebooks.

2. Before running the code make sure that the file 'memberList.json' is present within the current operating directory that should be the same directory as the application Python file.

3. The contained code will look for a file named 'memberList.json' within the starting directory it is operating in. 
  - An example input has been provided with the files of this project within the repository.

4. The application will use the scores of the current team members to determine what the combined score of the team is for each stat.

5. The application will then find the difference between this score and the maximum possible combined score of team to determine what stats the team is lacking the most. It will use this difference to determine the weight of importance for each stat to be used in applicant score calculations.

6. The application will multiply these weights by 10 and then sum them together to determine the maximum possible score for an applicant.

7. Each applicant will have their stats multiplied by their respecitve weight and then summed together to determine their overall score. 

8. Finally the overall score for each applicant will be divided by the maximum possible score an applicant could have to determine their final compatibility score.
  - For the sake of readibility due to possible close range of numbers the final compatibility scores are rounded to the second decimal value.

9. All results for each applicants final score are then stored in an object that will be written to an json file named 'app_scores.json' which will contain the final compatibility scores for each of the applicants. This file will be created as output within the current working directory.
