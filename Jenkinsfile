pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'g++ pipelinetest.cpp'
                echo "Build Successful!"
            }
        }
      stage('Test') {
        steps {
          sh './a.out'
          echo "Test Successful!"
        }
      }
      stage('Deploy') {
          steps {
        echo "Deploy Successful"
          }
      }
    }
    post {
        failure {
            echo "Pipeline failed!"
        }
    }
}
