
# Web Technologies Assignment 1 - HelloWorld Servlet 💖🚀

* - Still i faced some serverlet isuues but other thing working well ..  ⚠️⚠️

This assignment demonstrates how to run a simple HelloWorld Servlet program in VS Code using Java.

## Prerequisites

- [Java Development Kit (JDK)](https://www.oracle.com/java/technologies/javase-jdk11-downloads.html) installed on your system.
- [Visual Studio Code](https://code.visualstudio.com/) installed on your system.
- [Java Extension Pack](https://marketplace.visualstudio.com/items?itemName=vscjava.vscode-java-pack) installed in Visual Studio Code.
- Tomcat installation instruction given below at end *
## Setup

1. Clone or download the assignment repository to your local machine. or in vs code add `java extention package` after  `CTR + Shift + P` select gradle project press Enter.. it will create setup similler to this..

2. Open Visual Studio Code and navigate to the assignment folder.

## Instructions

1. Launch Visual Studio Code and open the assignment folder.
2. Install the required Java dependencies by following the instructions mentioned in the `Prerequisites` section.
3. Open the `src/main/java` directory.
4. Create a new Java class file named `HelloWorld.java`.
5. Copy and paste the following code into the `HelloWorld.java` file:

```java
import java.io.*;
import javax.servlet.*;
import javax.servlet.http.*;

public class HelloWorld extends HttpServlet {
    public void init() throws ServletException {
    }

    public void doGet(HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException {
        response.setContentType("text/html");
        PrintWriter out = response.getWriter();
        out.println("<h1> Hello World </h1>");
    }

    public void destroy() {
    }
}
```

<br/>

1. Save the file.
2. Right-click on the project folder and select "Run As" > "Run Configurations".
3. Click on the "Java Application" configuration type and then click on the "New launch configuration" button.( since proggram using serverlet for that i dounloaded tomcat server
4. Enter a name for the launch configuration and select the main class of the project (e.g., HelloWorld).
5. In the "Arguments" tab, add the following VM argument to specify the location of the Servlet API library:

7. 
```
-classpath <path/to/servlet-api.jar>
```
6. Replace `<path/to/servlet-api.jar>` with the actual path to your Servlet API library.
8. Click on the "Apply" button to save the launch configuration.

9. Right-click on the project folder again and select `"Run As" > "Java Application"` and select the launch configuration that you just created.

10. Once the application starts, open a web browser and type the URL of the Servlet in the address bar. The URL should be in the following format:
```http://localhost:8080/<web-app-name>/<servlet-name>```
11. Replace <web-app-name> with the name of your web application and `<servlet-name> `with the name of the Servlet class (e.g., HelloWorld).

12. Press Enter to send the request to the Servlet.

13. The Servlet should generate an HTTP response with the message "Hello World" in an HTML heading tag. The response should be displayed in the web browser.

<br/><br/>

 ###### Download Tomcat:
- * Visit the Apache Tomcat website at https://tomcat.apache.org/.
- * Click on the "Download" menu and select the version of Tomcat you want to install (e.g., Apache Tomcat 9).
- * Under the "Binary Distributions" section, click on the "32-bit/64-bit Windows Service Installer" link to download the .exe file.

 ###### Run the Installer:
* - Locate the downloaded .exe file and double-click on it to run the installer.
* - If prompted by User Account Control (UAC), click "Yes" to allow the installer to make changes to your system.

 ###### Choose Installation Options:
- The installer will open a setup wizard. Click "Next" to proceed.
- Read and accept the Apache Tomcat license agreement. Click "Next" to continue.
- Choose the destination folder where you want to install Tomcat. The default location is usually fine. Click "Next" to proceed.
- Select the components you want to install. By default, all components are selected, but you can customize the installation if desired. Click "Next" to continue. i added `port : 9494` for ensuring is not used anywhere so ,app manages access.
- Choose the Start Menu folder where the Tomcat shortcuts will be created. The default name is usually fine. Click "Next" to proceed.
- Select the additional tasks you want to perform, such as creating desktop shortcuts and running Tomcat as a service. Make your selections and click "Next" to continue.
- Review the installation summary and click "Install" to start the installation process.

 ###### Complete the Installation:
The installer will copy the necessary files and set up Tomcat on your system.
once the installation is complete, click "Finish" to exit the installer.

 ###### Start Tomcat:
- Open the Start menu and navigate to the Apache Tomcat folder.
- Click on the "Configure Tomcat" shortcut to open the Tomcat configuration tool.
- In the configuration tool, click on the "Tomcat" tab.
- Click on the "Start" button to start Tomcat.

 ###### Verify Tomcat Installation:
 - Open a web browser and enter the following URL:```http://localhost:9494```

If Tomcat is installed correctly, you should see the Tomcat welcome page.

<br/>
   
# Thanks for visiting to my repository 💖😍🌟.
  - if incase you like this repo please do stare 🌟 to this repository.
  - for this types of amzing contests do Visit Profile and Follow .  
  - if you want to constribute in this repo do it..PR i will happy to work with amazing people 😎.


  
  <br> <br> <br> <br> <br> <br> <br>
