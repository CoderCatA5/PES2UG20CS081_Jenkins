pipeline{
    agent any

    stages{
        stage('Clone Repository'){
            steps{
                git branch:'main',
                url : 'https://github.com/CoderCatA5/PES2UG20CS081_Jenkins.git'
            }    
        }
        stage('Build'){
            steps{
                sh 'make -C main'
            }
        }
        stage('Test'){
            steps{
                sh 'main/hello_exec oopsie'
            }
        }
        stage('Deploy'){
            steps{
        
                sh 'echo "Running file" && main/hello_exec'
            }
        }
    }
    post{
        failure{
            sh 'echo "Pipeline Failed"'
        }
    }
}