### ch.vorburger.exec
---
https://github.com/vorburger/ch.vorburger.exec

```java
ManagedProcessBuilder pb = new ManagedProcessBuilder("someExec")
  .addArgument("arg1")
  .setWorkingDirectory(new File("/tmp"))
  .getEnvironment().put("ENV_VAR", "...")
  .setDestoryOnShutdown(true)
  .addStdOut(new BufferedOutputStream(new FileOutputStream(outputFile)))
  .setConsoleBufferMaxLines(7000);

ManagedProcess p = pb.build();
p.start();
p.isAlive();
p.waitForExit();
p.exitValue()
String output = p.getConsole();

```

```
```

```
```
