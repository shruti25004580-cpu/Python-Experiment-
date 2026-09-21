#Aim:
#Write a Program to implement control flow statements and looping statements in python.

#Algorithm 

#1.Start.
#2.Store runs, balls, wickets, runs conceded, overs, and catches in lists.
#3.Use a for loop to process each player.
#4.Calculate Strike Rate.
#5.Calculate Economy Rate.
#6.Use if-elif-else to determine batting performance.
#7.Use if-elif-else to determine bowling performance.
#8.Use if-elif-else to determine fielding performance.
#9.Use if-elif-else to determine overall all-rounder category.
#10.Display the results.
#11.Repeat until all players are processed.
#12.Stop.

# CASE STUDY 1
# LOOPING + BRANCHING STATEMENTS

runs = [148, 179, 156, 117]
balls = [50, 62, 59, 41]
wickets = [4, 8, 6, 5]
runs_conceded = [29, 32, 29, 31]
overs = [2, 3, 4, 3]
catches = [3, 2, 2, 2]

for i in range(4):

    strike_rate = (runs[i] / balls[i]) * 100
    economy = runs_conceded[i] / overs[i]

    # Batting Performance
    if runs[i] >= 50 and strike_rate >= 120:
        batting = "Excellent Batter"
    elif runs[i] >= 30 and strike_rate >= 100:
        batting = "Good Batter"
    elif runs[i] >= 20:
        batting = "Average Batter"
    else:
        batting = "Poor Batter"

    # Bowling Performance
    if wickets[i] >= 3 and economy <= 6:
        bowling = "Excellent Bowler"
    elif wickets[i] >= 2 and economy <= 8:
        bowling = "Good Bowler"
    elif wickets[i] >= 1:
        bowling = "Average Bowler"
    else:
        bowling = "Poor Bowler"

    # Fielding Performance
    if catches[i] >= 2:
        fielding = "Outstanding Fielder"
    elif catches[i] == 1:
        fielding = "Active Fielder"
    else:
        fielding = "Needs Improvement"

    # Overall Performance
    if batting == "Excellent Batter" and bowling == "Excellent Bowler":
        overall = "Star All-Rounder"
    elif batting == "Good Batter" and bowling == "Good Bowler":
        overall = "Strong All-Rounder"
    elif batting == "Good Batter" or bowling == "Good Bowler":
        overall = "Supporting All-Rounder"
    else:
        overall = "Needs Improvement"

    print("\n-----------------------------")
    print("Player", i + 1)
    print("Strike Rate :", round(strike_rate, 2))
    print("Economy Rate:", round(economy, 2))
    print("Batting     :", batting)
    print("Bowling     :", bowling)
    print("Fielding    :", fielding)
    print("Overall     :", overall)
