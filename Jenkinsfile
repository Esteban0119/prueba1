pipeline {
  agent any
  stages {
    stage('Crear Archivo') {
      steps {
        script {
          def fecha = new Date().format("yyyy-MM-dd-HH-mm-ss")
          echo "'Hola Mundo' > ${fecha}.txt"
        }

      }
    }

  }
}