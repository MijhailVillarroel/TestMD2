# Running the tests
## Prerequisites
#### Step1 Install Gradle
- Please download the latest [Gradle](https://gradle.org/releases/) distribution
#### Step2 Unpack the distribution:
- Create a new directory **"C:\Gradle"** with File explore.
- Go to the directory where the Gradle distribution was downloaded. Double-click the ZIP archive to expose the content. Drag the content folder **gradle-verion** to your newly created **C:\Gradle folder**.
#### Step 3. Configure your system environment
- Configured the environment variable
-- then click `Properties` -> `Advanced System Settings` -> `Environmental Variables`.
-- Under `System Variables` select `Path`, then click `Edit`. Add an entry for `C:\Gradle\gradle-4...version\bin`. Click OK to save.
#### Step 4. Verify your installation
Open a console and run `gradle -v` to run gradle and display the version, e.g.:
```sh
$ gradle -v
------------------------------------------------------------
Gradle 4.8.1
------------------------------------------------------------
```
## Execute Gradle taks.
1. Run the following gradle task from the directory path where you clone the repository build.gradle file is located **e.g.**:
```sh
$ gradle cucumber -PcucumberOptions=@SalesOfficeDesignCenter
```
2. After completed cucumber gradle tasks, Run the following Gradle task:
```sh
$ gradle generateReport
```
3. Go to where you clone the repository `/build/cucumber-html-report`
4. Open the `index.html` report.