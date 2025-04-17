pipeline {
  agent any
  stages {
    stage('Clonar Repo') {
      steps {
        git url: 'https://github.com/Antonioedwardsd/integracion-continua.git', branch: 'master'
      }
    }
    stage('Instalar Dependencias') {
      steps {
        bat 'npm install'
      }
    }
    stage('Pruebas') {
      steps {
        bat 'npm run test'
      }
    }
  }
}
