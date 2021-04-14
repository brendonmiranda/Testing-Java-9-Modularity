Testing java 9 modularity feature

There is not much to see here, sorry 😂

Just a simple test 

### Run

### 1. Multi-module compilation: 
compile multiple modules with one javac command:

```
javac -d out --module-source-path "./*/src/" $(find . -name "*.java")
```

### 2. Execute modular application using module path

```
java --module-path out -m testA/com.test1.module.Test1Main
```

--module-path is the module path, its value is one or more directories that contain modules. The -m option specifies the main module, the value after the slash is the class name of the main class in the module


### References

https://openjdk.java.net/projects/jigsaw/quick-start

https://stackoverflow.com/questions/49476559/java-9-error-not-in-a-module-on-the-module-source-path

