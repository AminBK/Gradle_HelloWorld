# Gradle_HelloWorld
Testing new Gradle build referring to below:

https://spring.io/guides/gs/gradle/


======================
List of command:
======================

gradle build
gradle wrapper
.\gradlew run

======================
Command line execution
======================

C:\Java\SpringMvcHelloWorld>np build.gradle

C:\Java\SpringMvcHelloWorld>gradle build
:compileJava
C:\Java\SpringMvcHelloWorld\src\main\java\hello\HelloWorld.java:3: error: package org.joda.time does not exist
import org.joda.time.LocalTime;
                    ^
C:\Java\SpringMvcHelloWorld\src\main\java\hello\HelloWorld.java:7: error: cannot find symbol
    LocalTime currentTime = new LocalTime();
    ^
  symbol:   class LocalTime
  location: class HelloWorld
C:\Java\SpringMvcHelloWorld\src\main\java\hello\HelloWorld.java:7: error: cannot find symbol
    LocalTime currentTime = new LocalTime();
                                ^
  symbol:   class LocalTime
  location: class HelloWorld
3 errors
:compileJava FAILED

FAILURE: Build failed with an exception.

* What went wrong:
Execution failed for task ':compileJava'.
> Compilation failed; see the compiler error output for details.

* Try:
Run with --stacktrace option to get the stack trace. Run with --info or --debug option to get more log output.

BUILD FAILED

Total time: 4.563 secs

C:\Java\SpringMvcHelloWorld>ls
build  build.gradle  src

C:\Java\SpringMvcHelloWorld>np build.gradle

C:\Java\SpringMvcHelloWorld>echo %JAVA_HOME%
C:\Program Files\Java\jdk1.7.0_79

C:\Java\SpringMvcHelloWorld>gradle build
:compileJava
:processResources UP-TO-DATE
:classes
:jar
:assemble
:compileTestJava UP-TO-DATE
:processTestResources UP-TO-DATE
:testClasses UP-TO-DATE
:test UP-TO-DATE
:check UP-TO-DATE
:build

BUILD SUCCESSFUL

Total time: 9.674 secs
C:\Java\SpringMvcHelloWorld>
C:\Java\SpringMvcHelloWorld>
C:\Java\SpringMvcHelloWorld>
C:\Java\SpringMvcHelloWorld>gradle wrapper
:wrapper

BUILD SUCCESSFUL

Total time: 3.527 secs
C:\Java\SpringMvcHelloWorld>ls
build  build.gradle  gradle  gradlew  gradlew.bat  src

C:\Java\SpringMvcHelloWorld>./gradlew build
'.' is not recognized as an internal or external command,
operable program or batch file.

C:\Java\SpringMvcHelloWorld>chdir
C:\Java\SpringMvcHelloWorld

C:\Java\SpringMvcHelloWorld>chdir/gradlew build
The system cannot find the path specified.

C:\Java\SpringMvcHelloWorld>chdir\gradlew build
The system cannot find the path specified.

C:\Java\SpringMvcHelloWorld>.\gradlew build
Downloading https://services.gradle.org/distributions/gradle-2.3-bin.zip
...............................................................................................................................................................................................................................................................................................................................................................................................................................................................................................................................................................................................................................................................................................................................................................
...............................................................................................................................................................................................................................................................................................................................................................................................................................................................................................................................................................................................................................................................................................................................................................
.............................................................................................................................................................................................................................................................................................................................................................................................................................................................................................................................................................................................................................................................................
Unzipping C:\Users\IT-MEYO\.gradle\wrapper\dists\gradle-2.3-bin\a48v6zq5mdp1uyn9rwlj56945\gradle-2.3-bin.zip to C:\Users\IT-MEYO\.gradle\wrapper\dists\gradle-2.3-bin\a48v6zq5mdp1uyn9rwlj56945
:compileJava
:processResources UP-TO-DATE
:classes
:jar
:assemble
:compileTestJava UP-TO-DATE
:processTestResources UP-TO-DATE
:testClasses UP-TO-DATE
:test UP-TO-DATE
:check UP-TO-DATE
:build

BUILD SUCCESSFUL

Total time: 43.99 secs
C:\Java\SpringMvcHelloWorld>cd build

C:\Java\SpringMvcHelloWorld\build>ls
classes  dependency-cache  libs  tmp

C:\Java\SpringMvcHelloWorld\build>cd tmp

C:\Java\SpringMvcHelloWorld\build\tmp>cd jar

C:\Java\SpringMvcHelloWorld\build\tmp\jar>ls
MANIFEST.MF

C:\Java\SpringMvcHelloWorld\build\tmp\jar>ls
MANIFEST.MF

C:\Java\SpringMvcHelloWorld\build\tmp\jar>cd ..

C:\Java\SpringMvcHelloWorld\build\tmp>cd ..

C:\Java\SpringMvcHelloWorld\build>cd libs

C:\Java\SpringMvcHelloWorld\build\libs>ls
SpringMvcHelloWorld.jar  gs-gradle-0.1.0.jar

C:\Java\SpringMvcHelloWorld\build\libs>jar tvf gs-gradle-0.1.0.jar
     0 Tue Jan 12 09:24:40 SGT 2016 META-INF/
    25 Tue Jan 12 09:24:40 SGT 2016 META-INF/MANIFEST.MF
     0 Tue Jan 12 09:20:02 SGT 2016 hello/
   369 Tue Jan 12 09:24:40 SGT 2016 hello/Greeter.class
   988 Tue Jan 12 09:24:40 SGT 2016 hello/HelloWorld.class

C:\Java\SpringMvcHelloWorld\build\libs>cd ..

C:\Java\SpringMvcHelloWorld\build>cd ,,
C:\Java\SpringMvcHelloWorld\build

C:\Java\SpringMvcHelloWorld\build>cd ..

C:\Java\SpringMvcHelloWorld>cd ..

C:\Java>cd SpringMvcHelloWorld

C:\Java\SpringMvcHelloWorld>ls
build  build.gradle  gradle  gradlew  gradlew.bat  src

C:\Java\SpringMvcHelloWorld>.\gradlew run
:compileJava UP-TO-DATE
:processResources UP-TO-DATE
:classes UP-TO-DATE
:run
The current local time is: 09:29:39.208
Hello world!

BUILD SUCCESSFUL

Total time: 9.744 secs