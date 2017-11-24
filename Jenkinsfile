Jenkinsfile (Declarative Pipeline)
pipeline {
    agent { docker 'gradle:4.2.1' }
    stages {
        stage('build') {
            steps {
                sh 'gradle --version'
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
