pipeline{
    agent any
    stages{
        stage("Cleaun up"){
            steps{
                deleteDir()
            }
        }
        stage("Clone repo"){
            steps{
                sh "git clone https://github.com/qaziashfaq25/easybuggy-hd.git"
            }
        }
        stage("Build"){
            steps{
                dir("easybuggy-hd")
                    sh "mvn clean install"
            }
        }
        stage("Test"){
            steps {
                dir("easybuggy-hd")
                    sh "mvn test"
            }
        }
        }   
    }            
