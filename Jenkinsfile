pipeline {
    agent any
  stages {
    stage('Build') {
            steps {
                script {
                // some block
                    sh ./build.sh
                }
                //sh 'echo "Building..."'
                //sh 'ls -al'
            }
        }
      stage('Test') {
            steps {
                sh 'echo "Testing..."'
                sh 'pwd'
                sh 'touch testfile.txt'
                sh 'ls -l'
            }
        }
      stage('Deploy') {
            steps {
                sh 'cat ./run.sh'
                sh 'echo "Deploying..."'
                sh 'mv testfile.txt /tmp'
                sh 'ls -l /tmp'
            }
        }
  }
}
