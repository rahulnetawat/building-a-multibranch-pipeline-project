pipeline {
    agent any
    stages {
        stage('Develop Branch Build') {
            when {
                branch 'develop'
            }
            steps {
                sh 'echo "Hello from Develop Branch !!"'
            }
        }

        stage('Master Branch Build') {
            when {
                branch 'master'
            }
            steps {
                sh 'echo "Hello from Master Branch !!"'
                sh 'echo "Commit #1"'
            }
        }
        stage('Fix Branch Build') {
            when {
                branch 'fix-123'
            }
            steps {
                sh 'echo "Hello from Fix Branch !!"'
                sh 'echo "Commit #1 from Fix branch"'
            }
        }
  }
}
