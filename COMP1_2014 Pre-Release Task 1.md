#COMP1_2014 Pre-Release Tasks 

##Task 1

    def GetChoiceFromUser():
    Choice = input('Do you think the next card will be higher than the last card (enter y or n)? ')
	return Choice.lower()[0]


##Task 2

    def GetMenuChoice():
    Choice = input()
    print()
	return Choice.lower()[0]
	

##Task 3(a)
1. GetPlayerName( )
2. Using a while loop that continues until a name is entered
3. Instead of using an additional variable i would just initially set the variable PlayerName assigned to an empty string. This way a while loop that repeats until the variable is assigned to some actual text can be used.

###Pseudocode 
    	
    FUNCTION GetPlayerName():
	    PlayerName = String
	    PlayerName <-- ""
        WHILE PlayerName is equal to "" THEN
	        GET PlayerName
	        DISPLAY "Please enter your name: "
	        DISPLAY "" 
	   ENDWHILE     
	   RETURN PlayerName
###Program Code

    def GetPlayerName()
    print()
	playerName = ""
	while PlayerName == "":
		PlayerName = input('Please enter your name: ')
		print()
	return PlayerName

##Question 3(b)

1. PlayGame()

###Program Code

     NameChoice = input("Do you want to add your score to the high score table? (y or n): ")
      NameChoice = NameChoice.lower()[0]
      if GameOver:
        DisplayEndOfGameMessage(NoOfCardsTurnedOver - 2)
        if NameChoice == "y":
          UpdateRecentScores(RecentScores, NoOfCardsTurnedOver - 2)
      else:
        DisplayEndOfGameMessage(51)
        if NameChoice == "y":
          UpdateRecentScores(RecentScores, 51)

##Question 4

      def DisplayRecentScores(RecentScores):
      print()
      print('Recent Scores: ')
      print()
    
      print("{0:<10} {1:<10} {2:<10}".format("Name","Score","Date"))
      for Count in range(1, NO_OF_RECENT_SCORES + 1):
        print("{0:<10} {1:<10} {2:<10}".format(RecentScores[Count].Name,RecentScores[Count].Score,RecentScores[Count].Date))
      print()
      print('Press the Enter key to return to the main menu')
      input()
      print()


##Question 5
1. the datetime module
2.  - UpdateRecentScores()  
- DisplayRecentScores()
- ResetRecentScores()
- TRecentScore()
3. With the function datetime.strptime

##Additional Task - Variable Roles

|Role|Description|
|-----|--------------|
|Fixed Value|A variable that has a hard coded value that should not be changed|
|Stepper|A variable often used as a counter that is incremented or decremented usually to keep track of repetitions in while loops|
|Most Recent Holder|The most recent value interacted with by the program|
|Most Wanted Holder|A variable holding the most appropriate value attained thus far for the task|
|Gatherer|A variable containing the accumulative value of another set of variables|
|Transformation|A variable which has its value determined based on the values of other variables|
|Follower|A variable which has its value copied from another variable|
|Temporary|A variable which has a value that is only stored for a small amount of time|	

|Role|Example|
|-----|--------------|
|Fixed Value|NoOfSwaps = 1000|
|Stepper|Count = 1|
|Most Recent Holder|Choice = input('Do you think the next card will be higher than the last card (enter y or n)? ')|
|Most Wanted Holder|RecentScores[Count].Name = RecentScores[Count + 1].Name|
|Gatherer|NoOfCardsTurnedOver = 1|
|Transformation|NoOfCardsTurnedOver = NoOfCardsTurnedOver + 1|
|Follower| RecentScores[Count].Date = RecentScores[Count + 1].Date|
|Temporary|PlayerName = ""|


##Additional Task - Functions and Parameters

1. When passing by value the value of the variable that's called is copied to the functions parameter while when passing by reference a reference that directs the program to the correct memory location is passed as the parameter.

2.
|Function|Passing Mechanism|
|--------|-----------------|
|TCard|No Parameters|
|TRecentScore|No Parameters|
|GetRank|By Value|
|GetSuit|By Value|
|DisplayMenu|No Parameters|
|GetMenuChoice|No Parameters|
|LoadDeck|By Value|
|DisplayCard|By Reference|
|GetCard|By Refernce, By Value, By Value|
|IsNextCardHigher|By Value, By Value|
|GetPlayerName|No Parameters|
|GetChoicefromUser|No Parameters|
|DisplayEndOfGameMessage|By Value|
|DisplayCorrectGuessMessage|By Value|
|ResetRecentScores|By Reference|
|DisplayRecentScores|By Reference|
|UpdateRecentScores|By Reference, By Value|
|PlayGame|By Value, By Reference|


> Written with [StackEdit](https://stackedit.io/).

