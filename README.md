## How to use

#### Building JAR file

Checklist:
 * Build JAR file
   * Right click project name -> Export -> Java/Runnable JAR file -> Next
   * Select Main class
   * Select destination folder
   * Library handling: 3rd option
   
 * Pack files
   * JAR file
   * db.properties
   * MySQL Connector
   * JavaFX SDK
   * Java SDK
   
 ## Instalation
Checklist:
 * Install Java: https://www.oracle.com/technetwork/java/javase/downloads/index.html
   o Setup JAVA_HOME (ex: C:\Program Files\Java\jdk-11.0.3)
 * Copy JavaFX
   o Setup PATH_TO_FX (ex: C:\java-libs\javafx-sdk\lib)
   o Place MySQL Connector in lib folder
 * Copy JAR & db.properties
 
Run app:
java --module-path %PATH_TO_FX% --add-modules javafx.controls,javafx.fxml -cp myapp.jar
application.Main

## Bat File (optional)
java --module-path %PATH_TO_FX% --add-modules javafx.controls,javafx.fxml -cp myapp.jar
application.Main

## Windows Shortcut (optional)
Target:
"C:\Program Files\Java\jdk-11.0.3\bin\java.exe" --module-path %PATH_TO_FX% --add-modules
javafx.controls,javafx.fxml -cp myapp.jar application.Main

Start in:
C:\appfolder
