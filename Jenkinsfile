pipeline {
  agent any
  stages {
    stage('Crear Archivo') {
      steps {
        script {
          def fecha = new Date().format("yyyy-MM-dd-HH-mm-ss")
          def fileName = "${fecha}.txt"

          // Crear el archivo con el contenido deseado
          writeFile file: fileName, text: "Hola Mundo"

          // Imprimir la ubicación del archivo creado (opcional)
          echo "Archivo creado: ${fileName}"
          
         // Mover el archivo a otra carpeta
          bat "move \"${fileName}\" \"C:\\Users\\esteb\\OneDrive\\Desktop\\Trabajos Universidad\\Gestion\\Prueba3\\\""

         // Enviar correo electrónico
          emailext body: "Se ha creado el archivo ${fileName}",
                   subject: "Archivo creado",
                   to: "fargoz@gmail.com"


        }

      }
    }

  }
}
