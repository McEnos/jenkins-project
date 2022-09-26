pipeline{
    agent any
    stages{
        stage('build'){
            steps{
                echo 'Building the application............'
                sh "./gradlew build"
            }
        }
        stage('test'){
            steps{
                echo 'Testing the application............'
            }
        }
        stage('deploy'){
            steps{
                echo 'Deploying the application............'
            }
        }
    }
  /*   post{
        always{

        }
        success{

        }
        failure{

        }
    } */
}