# KurtNoe-Datahouse-Compatibility-Predictor
Code to take JSON files containing statistical scores of both a team and potential applicants. Takes these scores and uses them to calculate the compatibility of these applicants with the team to determine who is the best fit.

1. The contained code will look for a file named 'memberList.json' within the starting directory it is operating in. 
  - An example input for the JSON file contents will be provided at the bottom of this file, just in case.

2. Once the code finishes processing the data it will output a text file named 'app_scores.json' which will contain the final compatibility scores for each of the applicants.


Example Input for 'memberList.json': 
{
	"team":[
		{
			"name" : "Eddie",
			"attributes": {
				"intelligence": 1,
				"strength": 5,
				"endurance": 3,
				"spicyFoodTolerance": 1
			}
		}, {
			"name" : "Will",
			"attributes": {
				"intelligence": 9,
				"strength": 4,
				"endurance": 1,
				"spicyFoodTolerance": 6
			}
		}, {
			"name" : "Mike",
			"attributes": {
				"intelligence": 3,
				"strength": 5,
				"endurance": 9,
				"spicyFoodTolerance": 5
			}
		}
	],
	"applicants":[
		{
			"name" : "John",
			"attributes": {
				"intelligence": 4,
				"strength": 5,
				"endurance": 2,
				"spicyFoodTolerance": 1
			}
		},{
			"name" : "Jane",
			"attributes": {
				"intelligence": 7,
				"strength": 4,
				"endurance": 3,
				"spicyFoodTolerance": 2
			}
		},{
			"name" : "Joe",
			"attributes": {
				"intelligence": 1,
				"strength": 1,
				"endurance": 1,
				"spicyFoodTolerance": 10
			}
		}
	]
}
