pipeline{
    agent any
    tools {
      maven 'maven'
    }
    stages{
        stage('git'){
            steps{
                git credentialsId: 'jeevanchand0805', url: 'https://github.com/jeevanchand0805/myapp'
            }
        }
        stage('maven'){
            steps{
               sh 'mvn clean package'
            }
        }
    }
}
