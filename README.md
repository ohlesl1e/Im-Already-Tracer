# CSC690-Term-Project
Contact Tracing App

Contact Tracing iOS App

Overview: Uses location tracking in the iPhone to easily keep track of other phones that come     into a certain vicinity of the user. 

Features
Display a list of the (appleIDs?) of the other phones that user came in contact with
Modify list to output different data according to what the user wants (x days ago, etc)
Vicinity map 
Push notification tells user if they have come in contact with an infected individual and may need to quarantine. 
Keep track of any quarantine duration
Self report button => backend search other users in contact => notify them
Show the user locations they have been
Every 5 min, the app logs the location of the phone, using gps coordinates.
If a user reports themselves sick, the app will push notifications to all app users who have similar gps locations within a 100' radius cached in data, 
	
Model
	14 arrays of location	
View Controllers
	Create an Account VC:
		Connections:
		Action Button: Upload photo
		Action Button: Submit
		Text Field: Username
		Text Field: Password (hashed?)
		Label: Create an Account
		
		Functions:
		Action Button Clicked
		Upload Button Clicked
		
Backend 
	It handles self report and notify other users
	Node+MySQL(?)
