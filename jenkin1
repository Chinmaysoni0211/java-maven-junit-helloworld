pipline{
agent { label 'linux'}
options { 
buildDiscarder (logRotator(numToKeepStr: '5'))
}

stages{
    stage('Scan'){
steps {
with SonarQubeEnv(installationname: 'Sq1') {
sh '.mvnw clean org.sonarsource.scanner.maven:sonar-maven plugin:3.9.0.2155:sonar'
 }
 }
 }
 }
 }
