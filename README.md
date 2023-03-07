
* To reproduce issue #... , build this project excluding `exclude` module:

`apache-maven-3.9.0/bin/mvn -X -pl '!exclude' clean package`

Expected error: 

```
[ERROR] NullPointerException
java.lang.NullPointerException
at org.apache.maven.lifecycle.internal.MojoExecutor.executeForkedExecutions (MojoExecutor.java:439)
at org.apache.maven.lifecycle.internal.MojoExecutor.doExecute (MojoExecutor.java:325)
at org.apache.maven.lifecycle.internal.MojoExecutor.execute (MojoExecutor.java:213)
at org.apache.maven.lifecycle.internal.MojoExecutor.execute (MojoExecutor.java:175)
```