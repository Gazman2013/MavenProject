pipeline {
    agent any
  tools {
      maven 'localmvn'
  }
    stages {
        stage('Build') {
            input{
                message "are you hungry?"
                ok "Yes, I am"
                submitre "lex,jonh"
                parameters {
                    string(name: 'PERSON', defaultValue: 'Jenkins',
                           description: 'Description about qesstion')
                }
            }   
            steps {
                echo "Hello, ${PERSON}"
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                build job: 'checkstyle'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
