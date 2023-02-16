pipeline{
    agent any

    stages{
        stage('Clone Repository'){
            steps{
                git branch:'main',
                url : 'https://github.com/CoderCatA5/PES2UG20CS081_Jenkins.git'
            }    
        }
        stage('Clone Repository'){
            steps{
                git branch:'main',
                url : 'https://github.com/CoderCatA5/PES2UG20CS081_Jenkins.git'
            }    
        }
        stage('Build'){
            steps{
                make -C main
            }
        }
        stage('Test'){
            steps{
                main/hello_exec
            }
        }
    }
}