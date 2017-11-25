#!/usr/bin/env groovy
Jenkinsfile (Declarative Pipeline)
pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                echo './gradlew build'
            }
        }
    }
    post{
        success {
            echo 'El pipeline se ejecuto exitosamente'
        }
        failure {
            echo 'Ha ocurrido un error en la ejecucion del pipeline'
        }
        changed {
            echo 'El estado ha cambiado revisar'
        }
    }
}
