pipeline{
    agent any
    stages{
        stage('build'){
            steps{
                echo 'Building the application............'
                sh "./gradlew build -x test"
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
    post{
       success{
          archiveArtifacts 'build/libs/*.jar'
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