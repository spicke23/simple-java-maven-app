pipeline {
    agent any

    tools {
        maven 'jenkinsmaven'
    }

    stages {
        stage('Build') {
            steps {
                echo 'Realizando la clonacion del repo'
                git 'https://github.com/spicke23/simple-java-maven-app.git'
                echo 'Vamos a generar el repo'
                sh "mvn -Dmaven.test.failure.ignore=true clean package"
            }
        }
    }
}
