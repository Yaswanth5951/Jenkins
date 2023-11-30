pipeline {
    agent {label ""}
    environment {}
    tools{}
    parameters{}
    stages{
        stage("clean work space"){
            steps{
                cleanWs()
            }
        }
        stage( 'git checkout main ')
            steps{
               git url: 'https://github.com/Yaswanth5951/Jenkins.git' ,
                   branch: 'main'
            }
    }
    
}