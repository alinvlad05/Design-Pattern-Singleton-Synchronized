# Design-Pattern-Singleton-Synchronized
 
Using the synchronized keyword blocks access to the getInstance method by any new thread once a thread is executing code
inside the method;any new threads attempting to get in have to WAIT until the current thread is finished.
Using synchronized is one easy way to enforce single-threaded execution.

Warning:Synchronizing code involves a lot of overhead code that Java adds to MONITOR what's going on with threads.
And it slows your code down significantly for two reasons:
-The entrance to the synchronized method has to be constantly monitored,especially when a thread is inside the method executing code.
-Because synchronized code blocks threads to avoid conflicts, threads end up waiting for something to happen and losing your time.

Solution: Make sure the test isn't necessary at all.
Remove the object-creation code out of getInstance method completely.
See Design-Pattern-Singleton-Threaded
