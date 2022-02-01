pipeline {
  agent any
  stages {
    stage('Iniciando') {
      steps {
        echo 'New Pipeline'
      }
    }

    stage('Enviando mensagem') {
      steps {
        mail(subject: '[Jenkins] Iniciando esta pipeline', body: 'Iniciando a pipeline do testePratica5', replyTo: 'gabriel0603@alu.ufc.br', to: 'gabriel0603@alu.ufc.br')
      }
    }

  }
}