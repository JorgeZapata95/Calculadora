pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                bat './gradlew build'
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
