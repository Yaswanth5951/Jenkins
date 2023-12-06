pipeline {
    agent any
    stages{
        stage("clean work space"){
            steps{
                cleanWs()
            }
        }
        stage( 'git checkout main '){
            steps{
               git url: 'https://github.com/Yaswanth5951/spring-petclinic.git' ,
                   branch: 'main'
            }
        }
        stage("package clean"){
            steps{
                sh 'mvn clean'
            }
        }
        stage('package compile'){
            steps{
                script{
                    'mvn clean install'
                }
            }
        }
        stage('packages install'){
            steps{
                script{
                    'mvn clean package'
                }
            }
        }
    
    
    }
    
}
