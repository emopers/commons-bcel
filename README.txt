Running a console based verifier

   java org.apache.commons.bcel6.verifier.Verifier fully.qualified.class.Name

 lets JustIce work standalone.
 If you get a "java.lang.OutOfMemoryError", you should increase the
 maximum Java heap space. A command like

   java -Xmx1887436800 org.apache.commons.bcel6.verifier.Verifier f.q.c.Name

 will usually resolve the problem. The value above is suitable for
 big server machines; if your machine starts swapping to disk, try
 to lower the value.



Running a graphics based verifier

 If you prefer a graphical application, you should use a command like

   java org.apache.commons.bcel6.verifier.GraphicalVerifier

 to launch one. Again, you may have to resolve a memory issue depending
 on the classes to verify.


Contact

 If you spot a bug in the BCEL or its accompanying verifier "JustIce" please
 check with the BCEL mailing list

   http://commons.apache.org/bcel

 or enter the issue into the BCEL bug database

  https://issues.apache.org/jira/browse/BCEL
