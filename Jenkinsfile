pipeline {
  agent any
  stages {
    stage('Hola Mundo') {
      steps {
        echo 'Hola %miNombre%'
        sh 'printenv'
      }
    }

    stage('Crear archivo') {
      steps {
        writeFile(file: 'miArchvo.txt', text: 'Hola Mundo')
        archiveArtifacts '*.txt'
      }
    }

    stage('despedida') {
      steps {
        input(message: 'lastima que termino', ok: 'Excelente taller')
      }
    }

  }
  environment {
    miNombre = 'E017324'
  }
}