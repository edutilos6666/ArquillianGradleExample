```
//following commands are important for gradle arquillian project (in ArquillianGradleExample) : 
// find out linux flavor (Linux Centos from RedHat) 
cat /proc/version 

// find out centos version
cat /etc/centos-release


//following commands are important for gradle arquillian project (in ...) : 
//export wildfly server home 
export JBOSS_HOME=/home/aghayevn/wildfly-13.0.0.Final
//export gradle home 
export GRADLE_HOME=/home/aghayevn/Applications/gradle




//start gradle with proxy settings 
~/Applications/gradle/bin/gradle -s -Dhttp.proxyHost=100.100.101.58 -Dhttp.proxyPort=3128 clean test

//or we can add the following content into ~/.gradle/gradle.properties file: 
systemProp.http.proxyHost=100.100.101.58
systemProp.http.proxyPort=3128

systemProp.https.proxyHost=100.100.101.58
systemProp.https.proxyPort=3128

//and run gradlew 
./gradlew clean test
```


