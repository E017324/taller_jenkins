pipeline {
  agent any
  stages {
    stage('Hola Mundo') {
      steps {
        echo 'Hola printeven miNombre'
        sh 'printenv'
        sh '''echo "Hola "
printenv miNombre'''
      }
    }

    stage('Crear archivo') {
      steps {
        writeFile(file: 'miArchvo.txt', text: 'Hola Mundo')
        archiveArtifacts '*.txt'
      }
    }

  }
  environment {
    miNombre = 'E017324'
  }
}