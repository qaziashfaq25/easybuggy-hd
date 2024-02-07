pipeline {
    agent any
    tools{
        maven "Maven_3_5_2"
    }
    stages{
        stage('CompileandRunSonarAnalysis'){
            steps{
               sh 'mvn clean verify sonar:sonar -Dsonar.projectkey=hack-dossier-1 -Dsonar.organization=hack-dossier-1 -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=50c443b41f08f49a50f5fdd1aa25ce9c16c7ca75'
            }
            }
        }
    }

