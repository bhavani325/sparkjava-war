pipeline {
    agent any

    environment {
        PATH = "/opt/maven/bin:$PATH"
    }

    stages {
        stage('git clone') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/bhavani325/sparkjava-war.git'
            }
        }

        stage('build') {
            steps {
                sh 'mvn clean install'
            }
        }
    }
}
