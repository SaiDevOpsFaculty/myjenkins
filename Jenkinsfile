pipeline {
    agent any
    environment {
        PATH = "/opt/maven/bin:$PATH"
    }
    stages {
        stage('git clone') {
            steps {
                git url: 'https://github.com/SaiDevOpsFaculty/war-web-project.git', branch: 'master'
            }
        }
        stage('maven build') {
            steps {
                sh 'mvn clean install'
            }
        }
    }
}
