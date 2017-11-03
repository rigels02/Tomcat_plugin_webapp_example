Info Debugging with tomcat7:run
================================
Using Tomcat7 maven plugin. 


Debugging
------------------

### Easy way

1. go to project properties , selec Actions
2. from Actions select Goal and press button Add and from the displayed 
   list select: 'Debug maven build'.

### Other Way

    1.Open your console. 
    2.Navigate to your app folder.
    3.Start your app with mvnDebug (i.e. mvnDebug tomcat7:run, mvnDebug jetty:run)
    4. In NetBeans, select Debug->Attach Debugger
       Be sure to enter the following values, then click OK
         Debugger: Java Debugger (JDPA)
         Connector: SocketAttach (Attaches by socket to other VMs)
         Transport: dt_socket
         Host: localhost
         Port: 8000
    5. Go to you console window, and check if the app started.
    6. Add some breakpoints to you code.
    7. Open your app in your favorite browser.
    8. Navigate to the functionality you want to test.
