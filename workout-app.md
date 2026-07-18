## Workout Challenge App: Finding the Next Sensei

### Project Description
Once every three months, a Sensei rises. Born from hardship and lifting heavy ass weights, one individual rises above the rest. They stand tall amongst their peers with the knowledge that they are the superior lifter. 

A workout "app" was created using Google Sheets and Google Apps Script to facilitate a workout competition amongst friends. Competitors would be judged on four categories: Push, Pull, Legs, and Cardio. The person with the highest score at the end of the competition would be crowned the Sensei, and the others would live in shame (they would also need to do an amount of burpees depending on their placement).

### Project Overview
- Google Sheets was used since data storage and data visualization were straightforward, and the software was easily accessible to users. 
- Exercises were submitted using a Submission Form, which was operated using a script.
- Data was stored in one database and data calculations were done at the time of submission. 
- Data aggregation and analysis were done using formulas.


### Scoring
Scores were calculated by taking the total weight lifted per set divided by the user's bodyweight. Additionally, female competitors received a 33% bonus to scores. For example, if a female competitor weighed 120lbs and deadlifted 100 lbs for 5 reps, her score would be calculated as follows: 

$$
\frac{100lbs \times 5reps \times 1.33}{120lbs} = 5.54
$$ 

Exercises were divided amongst four categories: Push, Pull, Legs, and Cardio. The first three used the aforementioned formula, but cardio simply tracked time. 
<br>
Each exercise had additional metrics which could be incorporated into the score calculation, like difficulty modifier or bodyweight ratio. For example, the weight moved while doing certain exercises, like pushups, pullups, squats, etc., depends on the bodyweight of the individual. Approximate modifiers for each exercise were tested iteratively.

<img src="https://raw.githubusercontent.com/jamesbarber6406/workout-tracking-app/main/Screenshots/Leaderboard.png" alt="Workout App Leaderboard">

### Stats and Progression

Along with the leaderboard, users visualized exercise progression with plots and tables. The following are some examples of the visuals which were created during the competition:

<img src="https://raw.githubusercontent.com/jamesbarber6406/workout-tracking-app/main/Screenshots/Updating Progression Plots.png" alt="Progression Plots">

#### Stats Page for user E

<img src="https://raw.githubusercontent.com/jamesbarber6406/workout-tracking-app/main/Screenshots/Stats Dashboard%2C User E.png" alt="Stats Page">

## Submission Form

The submission form was designed to be simplistic and user-friendly. Cells use references and conditional formatting to make data input easy. The submission button uses a script which performs calculations on the input, clears the form, and outputs the data into a log. Fifteen rows were included to provide users flexibility when inputting data, beneficial if users were pyramiding sets or doing high weight/ low rep sets.

For more details, view the [script](https://github.com/jamesbarber6406/workout-tracking-app/blob/main/Submission%20Form.gs)

<img src="https://raw.githubusercontent.com/jamesbarber6406/workout-tracking-app/main/Screenshots/Submission Form.png" alt="Submission Form">
