pipeline {
  agent any
  stages {
    stage('Hola Mundo') {
      steps {
        echo 'Hola Mundo'
        sh 'printenv'
      }
    }

    stage('Crear archivo') {
      steps {
        writeFile(file: 'miArchvo.txt', text: 'Hola Mundo')
      }
    }

  }
}