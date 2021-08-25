echo "Main-Class: HangedUpThreads" > manifest.txt && javac HangedUpThreads.java && jar -cvfm HangedUpThreads.jar manifest.txt HangedUpThreads.class && native-image -H:EnableURLProtocols=http -H:EnableURLProtocols=https -H:ReflectionConfigurationFiles=reflection-config.json -jar HangedUpThreads.jar

./HangedUpThreads
