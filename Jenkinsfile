pipeline {
  agent any
  stages {
    stage('') {
      steps {
        sh '''pipeline {
    agent any

    stages {
        stage(\'Crear Archivo\') {
            steps {
                script {
                    def fecha = new Date().format("yyyy-MM-dd-HH-mm-ss")
                    sh "echo \'Hola Mundo\' > ${fecha}.txt"
                }
            }
        }
    }
}'''
        }
      }

    }
  }