
pipeline {
    agent any

    tools {
       
        maven "m3"
    }

    stages {
         stage("Clean Up"){
            steps {
                deleteDir()
            }
        }
        stage("Clone Repo"){
            steps {
               git 'https://github.com/anupanwa1/simple-maven-project-with-tests.git'
            }
        }
        stage("Build"){
            steps {
               
                    bat "mvn clean install"
                
            }
        }
    }
}
