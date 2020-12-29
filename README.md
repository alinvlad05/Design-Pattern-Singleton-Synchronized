# Design-Pattern-Singleton-Synchronized
 
Using the synchronized keyword blocks access to the getInstance method by any new thread once a thread is executing code
inside the method;any new threads attempting to get in have to WAIT until the current thread is finished.
Using synchronized is one easy way to enforce single-threaded execution.
