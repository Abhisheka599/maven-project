pipeline {
    agent any 
    stages {
        stage('scm checkout') {
            steps {
                git branch: 'master' , url: 'https://github.com/Abhisheka599/maven-project/'
            }
        }
        stage ('compile source code'){
             steps {
                 maven(jdk: 'localjava', maven:'localMaven') {
                     sh 'mvn compile'
                 }
             }
        }
        }
}
