pipeline {
  agent any
  stages {
    stage('Iniciando') {
      steps {
        echo 'Building Pipeline'
      }
    }

    stage('Enviando mensagem') {
      steps {
        mail(subject: '[Jenkins] Pipeline Pratica 5', body: 'Iniciando a pipeline do testePratica5', replyTo: 'gabriel0603@alu.ufc.br', to: 'gabriel0603@alu.ufc.br')
      }
    }

    stage('Teste') {
      steps {
        sleep 15
        build(propagate: true, job: 'UnicornTest')
        mail(subject: 'Iniciando teste', body: 'Prática 5 concluída', to: 'gabriel.raulino@alu.ufc.br')
      }
    }

  }
}