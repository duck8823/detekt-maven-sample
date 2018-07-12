```bash
$ mvn verify
```

```
[INFO] Scanning for projects...
[INFO] ------------------------------------------------------------------------
[INFO] Reactor Build Order:
[INFO] 
[INFO] detekt-maven-sample                                                [pom]
[INFO] module1                                                            [jar]
[INFO] module2                                                            [jar]
[INFO] 
[INFO] --------------< detekt-maven-sample:detekt-maven-sample >---------------
[INFO] Building detekt-maven-sample 0.0.1-SNAPSHOT                        [1/3]
[INFO] --------------------------------[ pom ]---------------------------------
[INFO] 
[INFO] --------------------< detekt-maven-sample:module1 >---------------------
[INFO] Building module1 0.0.1-SNAPSHOT                                    [2/3]
[INFO] --------------------------------[ jar ]---------------------------------
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ module1 ---
[WARNING] Using platform encoding (UTF-8 actually) to copy filtered resources, i.e. build is platform dependent!
[INFO] Copying 0 resource
[INFO] 
[INFO] --- maven-compiler-plugin:3.1:compile (default-compile) @ module1 ---
[INFO] Nothing to compile - all classes are up to date
[INFO] 
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ module1 ---
[WARNING] Using platform encoding (UTF-8 actually) to copy filtered resources, i.e. build is platform dependent!
[INFO] skip non existing resourceDirectory /Users/duck8823/Repositories/detekt-maven-sample/module1/src/test/resources
[INFO] 
[INFO] --- maven-compiler-plugin:3.1:testCompile (default-testCompile) @ module1 ---
[INFO] Nothing to compile - all classes are up to date
[INFO] 
[INFO] --- maven-surefire-plugin:2.12.4:test (default-test) @ module1 ---
[INFO] No tests to run.
[INFO] 
[INFO] --- maven-jar-plugin:2.4:jar (default-jar) @ module1 ---
[INFO] 
[INFO] --- detekt-maven-plugin:1.0.0.RC7-3:check (default) @ module1 ---
[INFO] Args:


0 kotlin files were analyzed.


Project Statistics:
        - number of properties: 0
        - number of functions: 0
        - number of classes: 0
        - number of packages: 0
        - number of kt files: 0

Successfully generated HtmlOutputReport at /Users/duck8823/Repositories/detekt-maven-sample/module1/detekt/detekt-report.html
Successfully generated XmlOutputReport at /Users/duck8823/Repositories/detekt-maven-sample/module1/detekt/detekt-checkstyle.xml
Successfully generated PlainOutputReport at /Users/duck8823/Repositories/detekt-maven-sample/module1/detekt/detekt-plain.txt

detekt finished in 1115 ms.
[INFO] 
[INFO] --------------------< detekt-maven-sample:module2 >---------------------
[INFO] Building module2 0.0.1-SNAPSHOT                                    [3/3]
[INFO] --------------------------------[ jar ]---------------------------------
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ module2 ---
[WARNING] Using platform encoding (UTF-8 actually) to copy filtered resources, i.e. build is platform dependent!
[INFO] Copying 0 resource
[INFO] 
[INFO] --- maven-compiler-plugin:3.1:compile (default-compile) @ module2 ---
[INFO] Nothing to compile - all classes are up to date
[INFO] 
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ module2 ---
[WARNING] Using platform encoding (UTF-8 actually) to copy filtered resources, i.e. build is platform dependent!
[INFO] skip non existing resourceDirectory /Users/duck8823/Repositories/detekt-maven-sample/module2/src/test/resources
[INFO] 
[INFO] --- maven-compiler-plugin:3.1:testCompile (default-testCompile) @ module2 ---
[INFO] Nothing to compile - all classes are up to date
[INFO] 
[INFO] --- maven-surefire-plugin:2.12.4:test (default-test) @ module2 ---
[INFO] No tests to run.
[INFO] 
[INFO] --- maven-jar-plugin:2.4:jar (default-jar) @ module2 ---
[INFO] 
[INFO] --- detekt-maven-plugin:1.0.0.RC7-3:check (default) @ module2 ---
[INFO] Args:
Can only specify option -i once.

Usage: detekt [options]
  Options:
    --baseline, -b
      If a baseline xml file is passed in, only new code smells not in the 
      baseline are printed in the console.
    --config, -c
      Path to the config file (path/to/config.yml).
    --config-resource, -cr
      Path to the config resource on detekt's classpath (path/to/config.yml).
    --create-baseline, -cb
      Treats current analysis findings as a smell baseline for future detekt 
      runs. 
      Default: false
    --debug
      Prints extra information about configurations and extensions.
      Default: false
    --disable-default-rulesets, -dd
      Disables default rule sets.
      Default: false
    --filters, -f
      Path filters defined through regex with separator ';' (".*test.*").
    --generate-config, -gc
      Export default config to default-detekt-config.yml.
      Default: false
    --help, -h
      Shows the usage.
  * --input, -i
      Input paths to analyze.
    --output, -o
      Directory where output reports are stored.
    --output-name, -on
      The base name for output reports is derived from this parameter.
    --parallel
      Enables parallel compilation of source files. Should only be used if the 
      analyzing project has more than ~200 kotlin files.
      Default: false
    --plugins, -p
      Extra paths to plugin jars separated by ',' or ';'.
    --print-ast
      Prints the AST for given [input] file. Must be no directory.
      Default: false
    --run-rule
      Specify a rule by [RuleSet:Rule] pattern and run it on input.
```
