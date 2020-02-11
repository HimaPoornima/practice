# Steps to install Apache Jmeter and Run the Application
##### 1.Install Java
 - JMeter is pure Java desktop application, it requires a fully compliant JVM 8 or higher. You can download and install the latest version of Java SE Development Kit from link given below
 https://www.oracle.com/technetwork/java/javase/downloads/index.html. 
##### 2.Download Jmeter  
- Install apache-jmeter-5.1.1.zip from https://jmeter.apache.org/
##### 3.Installation
- You can simply unzip the zip/tar file (which is downloaded from above mentioned link) into the directory where you want JMeter to be installed.
##### 4.Running  and Launching Jmeter
- After installation is completed,go to unzipped folder and then go to bin directory
- Now, run jmeter.bat file (to run it in GUI mode)

#
#
Jmeter window in GUI mode
<<<<<<< HEAD
 ![Jmeter window](/test/screenshots/ApacheJmeterSnap.png)
=======
 ![Jmeter window](/screenshots/ApacheJmeterSnap.png)
>>>>>>> 4af58db745c32742e568fd4831ed911ab93cf4f6


# Create and Run a new Test Plan in Jmeter

  - Right click on test plan in left test plan pane and add Threads->ThreadGroup
  - Inside thread properties of ThreadGroup element enter the Number of Threads,Ramp-up period,Loop count values.
  - Right click on ThreadGroup->ConfigElement->HTTP HeaderManager (which is used to store headers and is optional).
  - Right click on ThreadGroup->Add->Sampler->HTTPRequest 
      - In the HTTP Request, mention all the details of Severname/IP,portnumber,Protocol,path,HTTP Method. In case if post method is used then enter details in bodydata.
  - Right click on HTTPRequest->Add->Listner->View Results Tree
  - Right click on HTTPRequest->Add->Listner->View Results in Table
  - Right click on HTTPRequest->Add->Listner->Summary Report
  - After adding all the components & before running a test, you should save your Test Plan first. 
    - Go to File -> Save Test Plan as-> a Dialog box display
    - Enter a filename of Test Plan ->click Save (save it in .jmx format)
  - Then, start executing the TestPlan by clicking start button.

# How to run an existing JMX file

  - Open Jmeter Gui window and Go to File menu->Open (select the jmx file that you want to run).
  - Already existing file has the data to be posted and port numbers according to which mentioned in application.properties.
    - Note: Before running the test plan,make sure to change the port numbers in HTTP Request Sampler if you are using different ports.
  - Run the testplan as shown in below screenshot.
<<<<<<< HEAD
  ![Jmeter window](/test/screenshots/RunTestPlan.png)
=======
  ![Jmeter window](/screenshots/RunTestPlan.png)
>>>>>>> 4af58db745c32742e568fd4831ed911ab93cf4f6
  - Results can be viewed in TestPlan after running it.
  
# Performance comparison of Vert.x and Springboot

<<<<<<< HEAD
For more information, refer to the word document which is added in the folder test 
=======
For more information, refer to the word document which is added in the folder test 

>>>>>>> 4af58db745c32742e568fd4831ed911ab93cf4f6
