# Election Analysis

## Project Overview

We have been hired by a Colorado Board of Elections employee to calculate and analize the result of voter data from a recent local congressional elections.

1. Calculate the number of votes cast.
2. Compile a list of all candidates who received votes.
3. Calculate the number of votes each candidate received.
4. Caclulate the precentage of votes each candidate received.
5. Determine the winner of the election based on the popular vote.

## Resources:

Data Source: elections_data.csv
Software: Python 3.6.1, Visual Studio Code 1.38.1

## Results:
* There were 369,711 votes cast
* Voting by district:
  * Jefferson had 10.5% of the votes and 38,855 ballots cast.
  * Denver had 82.8% of the votes or 306,055 voters.
  * Arapahoe had 6.7% of the votes ord 24,801 voters.
* Denver had the largest turnout with 82.8% of the votes or 306,055 voters.
* Candidates were: Charles Casper Stockham, Diana DeGette, Raymon Anthony Doane
* Candidate results:
  * Stockham- 23.0% / 85,213 votes
  * DeGette- 73.8% / 272,892 votes
  * Doane- 3.1% / 11,606 votes
* Winner is Diana Degette who received 73.8% of the vote for a total of 272,892 votes

## Election- Audit Summary:
* This project can be used for any future elections as long as the data similarly structured. The structure should be: Ballot ID | County | Candidate. 
* We can modify the PyPoll_Challenge.py script by assigning user input variables for the folder and name of the results *.csv file and analysis *.txt file. to do so, change the script from:
#### # Add a variable to load a file from a path.
file_to_load = os.path.join("Resources", "election_results.csv")
#### # Add a variable to save the file to a path.
file_to_save = os.path.join("analysis", "election_analysis.txt")

to:

#### # Ask User to enter the folder and file name of the results *.csv file to read
file_to_load_location = input("Enter the name of the folder containing the results *.csv file please.  ")
file_to_load_name = input("Enter the name of the results *.csv file please.  ")
#### # Add a variable to load a file from a path.
file_to_load = os.path.join(file_to_load_location, f"{file_to_load_name}.csv")

#### # Ask User to enter the folder and file name of the analysis *.txt file to create/save
file_to_save_location = input("Enter the name of the folder containing the analysis *.txt file please.  ")
file_to_save_name = input("Enter the name of the analysis *.txt file please.  ")
#### # Add a variable to save the file to a path.
file_to_save = os.path.join(file_to_save_location, f"{file_to_save_name}.txt")


