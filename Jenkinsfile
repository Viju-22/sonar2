pipeline
{
    agent any
    stages{
        stage('Build Application'){
        steps{
        bat 'mvn -X clean package -DskipTests'
        }
       
        }
       
        stage('SonarQube Testing'){
        steps{
        bat 'mvn sonar:sonar -Dsonar.sources=src/ -Dsonar.host.url=http://localhost:9000 -Dsonar.login=c91a76d35e003f1d1af99856195a65522c327514'
            }
        }
       
   
    }
}
