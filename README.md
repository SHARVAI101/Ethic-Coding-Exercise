# Ethic-Coding-Exercise
Created by Sharvai Patil (sp4479@g.rit.edu)

## How to run:
1. Unzip the zip file and open a command prompt in the solution folder and execute the following commands:<br>
	a. gradlew build<br>
	b. gradlew run --args='filename of the .txt file with path' (eg. gradlew run --args='D:\testing.txt' OR gradlew run --args='"D:\Ethic Test\testing.txt"' OR gradlew run --args='"../../testing.txt"') 
3. IMPORTANT NOTE: If you are entering a relative path, the path has to be relative to the lib folder(so for a file in the lib folder, the path would be "myfile.txt"). To reduce complexity, I recommend giving an absolute path as an argument.
4. To run the unit tests, execute the following command:<br>
	gradlew test<br>
	If you get a message that says "BUILD SUCCESSFUL" that means all tests passed.<br>
	If you get a message that says "BUILD FAILED" along with a java.lang.AssertionError, that means some test cases failed.<br>

## Assumptions considered:
1. Palindrome checks are case insensitive (i.e, kayak and Kayak are both considered to be palindromes)
2. Only numbers are also considered as words e.g., "abc 12 hi" are counted as 3 words.
3. Groups of only special characters are not considered as words e.g., "%$@" is not considered to be a word

## Miscellaneous notes:
1. lib/src/test/resources has 2 test files that are being used for testing. You can also use these files for testing. For the same, use the following commands:<br>
gradlew run --args="src/test/resources/testing.txt"<br>
gradlew run --args="src/test/resources/testing2.txt"
