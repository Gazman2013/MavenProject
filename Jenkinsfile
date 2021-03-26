pipeline {
    agent any
    tools {
        maven 'localmvn'
    }
    stages {
        stage('Build') {
            input {
                message "are you hungry?"
                ok "Yes I am"
                submitrer "lex,john"
                parameters {
                    string(name: 'PERSON', defaulValue: 'Jenkins',
                           description: 'Description about qesstion')
                }
                steps
            steps {
                echo "Hello"
                sh 'mvn --version'
                echo 'Building2..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                build job:'checkstyle'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
