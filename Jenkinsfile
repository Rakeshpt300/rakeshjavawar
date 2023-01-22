pipeline {
    agent any
    stages { 
        stage('git') {
            steps {
                echo 'this is the git stage to clone repo'
                git branch: 'main', url: 'https://github.com/Rakeshpt300/rakeshjavawar.git'
            }
        }
        stage('mavenBuild') {
            steps {
                sh 'mvn clean install'
            }
            }
        stage('deploytomcat') {
            steps {
               echo 'this is the deploy stage'
            }
            }
        stage('test') {
            steps {
               echo 'this is the test stage'
            }

        }
    }
}

