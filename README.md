
--------------------------------------------------
----------INTRODUCTION
--------------------------------------------------

Thanks for taking the time to check out this little work sample of mine.
Provided within this document are instructions for compiling the project from source and running the compiled code.
My class which you'll be interested in examining is App.java, found here: slcsp/src/main/java/com/mycompany/slcsp/slcsp/App.java.
Please enjoy exploring my code.

This example constitutes a Java program I've written which modifies a file named slcsp.csv.
For a detailed explanation of this problem, as it was presented for me to solve, please see slcsp/data-resources/readme.md.
Otherwise, a very concise summary of the problem can be found below.

Concise summary of problem:
The spreadsheet slcsp.csv is intended to display a list of zip codes, along with a corresponding insurance rate for each zip code.
The spreadsheet has two columns: one for zip code; and one for rate. The rate column is currently empty.
The purpose of my Java program is to determine the rate for each zip code and thus populate the rate column, leaving a blank cell if there is not enough information to determine the rate.
In order to determine the rates, my program takes information into consideration from two other .csv files: plans.csv; and zips.csv.

slcsp.zip contains the original version of slcsp.csv, in slcsp/data-resources directory, and will modify this once the app runs.
Once modified, slcsp/data-resources/slcsp.csv should match, exactly, the finished version of slcsp.csv that I have included outside of the slcsp directory.

The contents of this work sample are:
 This comments file
 A finished version of slcsp.csv
 slcsp.zip (my app)

* Windows is not recommended for viewing this work sample.

--------------------------------------------------
----------INSTALLATION INSTRUCTIONS FOR MAC USERS
--------------------------------------------------

[A] -- INSTALL MAVEN

1. Run this command in a command line terminal: "sudo apt-get install mvn".
(If this does not work, try "sudo apt-get install maven".)

2. Verify Maven installation with this command: "mvn -version".
Output ought to be similar to this:
"Apache Maven 3.0.5
Maven home: /usr/share/maven
Java version: 1.7.0_55..."

[B] -- COMPILE PROJECT

1. Unzip slcsp.zip.

2. Open a command line terminal within the "slcsp" directory which you have unzipped.
To ensure you are in the correct directory, run the "ls" command, then ensure pom.xml is among the files listed.

3. Run this command: "mvn compile assembly:single".

[C] -- RUN COMPILED PROGRAM

1. From a command line terminal within the unzipped "slcsp" directory, run the command "cd target" to navigate into the "target" directory.

2. Run the jar file by running this command: "java -jar slcsp-0.0.1-SNAPSHOT-jar-with-dependencies.jar".
And -voila- you have successfully run the application.

