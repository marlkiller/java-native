# introduce
java native sample project
Build with maven/gradle


# env
- graalvm-jdk-17 (https://github.com/graalvm/graalvm-ce-builds/releases)
- maven|gradle

# build run
## native-image
```jshelllanguage
native-image -cp ./target/java-native-0.0.1-SNAPSHOT.jar -H:Name=helloworld -H:Class=Demo -H:+ReportUnsupportedElementsAtRuntime --allow-incomplete-classpath
```

## mvn
```jshelllanguage
mvn package
./target/java-native
```

## gradle
```jshelllanguage
gradle -x test clean build nativeCompile
./build/native/nativeCompile/java-native
```


