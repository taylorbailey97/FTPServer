# FTP Server

This is a sample FTP server program that allows the a user to add send a file through an HTTP Post request, update the file, and use a GET request to download the file.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

You'll need to have the following installed before running the server
* [JDK](https://www.oracle.com/java/technologies/javase-downloads.html) - JDK 1.8 or above
* [Maven](https://maven.apache.org/download.cgi) - Maven 3.2+
* [Git](https://git-scm.com/downloads) - Git for the command line (optional)

### Installing

First clone the repository into a directory on your computer. You do this starting from the command line, move to a folder that you would like to have the files stored at. for example: YourRootDirectory/documents. Use the command below to clone it. If you would like to avoid cloning the repository you can download the files directly [Here](https://github.com/taylorbailey97/FTPServer/archive/master.zip)

```
git clone https://github.com/taylorbailey97/FTPServer.git
```

### Running the server

Follow the steps below to get the server up and running

From a command line change into the root directory of the files that you cloned or downloaded earlier. Using cd to change directories like the command below:

```
cd yourPathToFolderHoldingFiles/FTPServer
```

Once you're in the servers root folder for files run the following command. NOTE: you may be prompted for permission for Java to access your computer, this is fine allow Java to do so.

```
./mvnw spring-boot:run
```

There will be server informational items that pop up on the command line, once it stops outputting information move over to a browser and enter in the search bar at the top of the browser to localhost:8080 or click [here](localhost:8080)

### Testing the server

After you open up localhost:8080 you'll be directed to a sample html page that has two buttons at the top "Choose File" and "Upload". 

#### Uploading a file
  1. Click the "Choose File" button and select a file from your system in the pop up window
  
  2. Click the "Upload" button, you should see at the top of the screen a success message saying that the file was uploaded
     successfully
     
  3. A list will appear on the webpage with the file you've just uploaded
  
  NOTE: Repeat these steps as many times as you'd like adding more and more files to the server
  
#### Downloading a file
  NOTE: There must be at least one file already uploaded to the server before you can download one
  
  1. Select a file from the list of files that are displayed on the sample webpage loaded up on localhost:8080
  
  2. Click on the blue hyperlink for that file and select a location for the file to download
  
  3. The file will begin downloading and you'll be able to access that file from your computer
  
#### Updating a file
  In order to update a file you reupload the same file, so if you wanted to update examplefile.txt you would use the 
  steps in uploading a file and select examplefile.txt.
  
#### Deleting a file
  NOTE: There must be at least one file already uploaded to the server before you can download one
  
  1. Select a file from the list of files that are displayed on the sample webpage loaded up on localhost:8080
  
  2. Click on the black hyperlink for that file and that says "Delete"
  
  3. The file will be deleted

## Authors

* **Taylor Bailey** - *Initial work* - [Github](https://github.com/taylorbailey97)

## Acknowledgments

* [Spring.io](https://spring.io/) - has been helpful with documentation and tutorials with getting started with Spring Boot
