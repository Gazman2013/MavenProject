pipeline {
    agent any
  tools {
      maven 'localmvn'
  }
    stages {
        stage('Build') {
            steps {
                sh 'mvn --version'
                echo 'Building1..'
                echo 'Building2..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
