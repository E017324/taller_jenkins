pipeline {
  agent any
  stages {
    stage('Hola Mundo') {
      steps {
        echo 'Hola Mundo'
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