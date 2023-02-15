pipeline {
    agent any
    tools {
        maven 'maven3'
        jdk 'jdk8'
    }
   
    stages{
        stage('git Repo Pull'){
            steps{
                sh 'git --version'
                sh 'whereis git'
                git 'https://gitlab.com/renukamusuluri1981/automaticdeployment.git'
            }
        }
        stage('maven clean'){
            steps{
                sh 'mvn clean'
                sh 'mvn install'
            }
        }
    }
}
