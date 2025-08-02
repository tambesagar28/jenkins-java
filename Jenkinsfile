pipeline{
    agent any

    environment{
        RELEASE_VERSION='2.1'
         
    }
    stages{

        
        stage('build'){
            steps{
                sh 'mvn clean package'
            }
        }

        stage('Test'){
            steps{
                sh 'echo "test command"'
            }
        }

        stage('Deploy'){
            steps{
                sh 'echo "deploy command"'
            }
        }
    }
}

    post{
        success{
            echo 'Pipeline succeeded!'
        }
        failure{
            echo 'Pipeline Failed!'
        }
    }