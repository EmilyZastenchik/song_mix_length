# song_mix_length
Assignment 4 Intro programming 1

Assignment 4
Emily Zastenchik

Software Development Method
PROBLEM: Asks user for song title and length.  After each input the program displays 
the last song input and the current length of mix. (Note: add 5 seconds in between each song).
After the user has finished entering all of the songs, the program outputs the total length of song mix in minutes and seconds.

ANALYSIS:
	Constant:
	SENTINEL = "DONE"
	Inputs:
		string title;	//song title 
		string restOfLine; 
		int length;		//song length
		int sum;		//sum of songs in seconds
		
	Outputs:
	"After adding ____________, your song mix is ___________ seconds long."
	"Your final mix will be _____ minutes and _____ seconds."
	Error message for negative song length values (use if statement)
	
	Functions:
		********getline(cin, restOfLine, '\n') / [title.insert(title.length(), restOfLine)]******
		int findMin(int)		//pass total length in seconds and return minutes value
		int findSeconds(int)		//pass total length in seconds and return seconds value
		
	Loop:
	while(length >= 0)
	if(title != SENTINEL)
		
DESIGN:
	Display message/directions for program
	Loop with SENTINEL
		Ask user for first song title, store in string title (use member function to cin song title)
		Ask user for song length in seconds, store value in int length
		Add 5 seconds in between each entered song length, and acculmulate song length in int length
		Display last song title input and current mix length
		("After adding ____________, your song mix is ___________ seconds long.")
	Pass int length to findMin and findSeconds functions
	
	After user has entered SENTINEL value to exit loop, output: "Your final mix will be _____ minutes and _____ seconds."
