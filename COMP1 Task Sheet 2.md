
##Task 6
1.  It should be recorded in the main section of the program.
2. DisplayMenu( )
3. IsNextCardHigher(LastCard, NextCard)

###Pseudocode

    Function DisplayOptions()
	    OUT "OPTION MENU"
	    OUT "1. Set Ace To High Or Low"
	    GetOptionChoice()

    Function GetOptionChoice()
	    WHILE OptionChoice = "" THEN
		    OUT "Please Enter Option: "
		    GET OptionChoice 
		ENDWHILE

    Function SetOptions(OptionChoice)
	    IF OptionChoice = 0 THEN
		    OUT ""
		    ENDIF
		IF OptionChoice = 1 THEN
			 SetAceHighOrLow()
		ENDIF
		return AceValue
		
    Function SetAceHighOrLow()
	    OUT "Would you like to set Ace to high(h) or low(l)? "
	    AceValue = UserInput.lower()[0]
	    


	    
##Task 7 

###PseudoCode

       Function ArrangeScores(RecentScores):
          end <-- True
          Length <--- len(RecentScores)
          WHILE end = true THEN
              Length <-- Length - 1
              end <-- False
              for range(1,Length-1) THEN
                  IF RecentScores[item].Score < RecentScores[item+1].Score THEN
                      placeHolder = RecentScores[item+1]
                      RecentScores[item+1] = RecentScores[item]
                      RecentScores[item] = placeHolder
                      end <-- true
                      ENDIF
                ENDWHILE
                     
##Task 8


 
 
  

> Written with [StackEdit](https://stackedit.io/).

