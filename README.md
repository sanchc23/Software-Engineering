# Software Engineering

This is the coding work for ECE/CS 506- Software Engineering at UW-Madison.

The class was made to mimic an authentic software engineering environment, working on one big project in 2 week agile sprints.

I worked on a team of 8 engineers, and our project was the UltaTracker, which is an Android application that is meant to serve as a Health/Exercise tracker and a planner simultaneously.  

Taken in the Spring of 2021.
 
Instructions for Running the UltaTracker:

1. Navigate to the Github repository for the UltaTracker: https://github.com/sanchc23/ECE-556-Software-Engineering

2. Navigate to the Iteration 2 release, found along the right side of the main repository page.  Download the .zip file.  Extract it somewhere to come back to later.

3. If Android Studio is not already downloaded, download it: https://developer.android.com/studio

4. Open the extracted UltaTracker project in Android Studio.  

5. Some members of the team had issues running the project without manually building APKs.  As a precaution, in Android Studio along the top bar, click Build -> Build Bundle(s) / APK(s) -> Build APK(s).

6. To Run the App on the Android Emulator, Click the Green Play Button on the top of Android Studio
	- Alternatively, you can click the Run button along the top bar, and select "Run 'app'".

7. To Run all tests:

	- Open up the Android emulator
	
	- Delete the Current UltaTracker App on the Emulator by hitting the home button on the emulator, swiping up to the app menu. Then, hold down on the app icon and drag to uninstall. 
	  This is to ensure the correct state of the app during UI tests. 
	
	- Navigate to the Gradle Wrapper(click the Gradle Elephant along the right side of Android Studio)
	
	- On the directory located along the left side, click on the Folder UltaTracker/Tasks/reporting and double click the createTestReport item to run the test reports.
		
		- Alternatively, if you click on the build.gradle(:app) file and go to line 93 the tests suite can be ran by clicking on the play button located there.
		
	- The reports can be found at the following locations
		
		- Unit Tests: UltaTracker/app/build/reports/test/testDebugUnitTest/index.html
		
		- UI/Integration Tests: UltaTracker/app/build/reports/androidTests/connected/flavors/debugAndroidTest/index.html
				
		- Code Coverage: UltaTracker/build/coverage-report/index.html
