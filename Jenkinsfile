pipeline {
  agent any
  stages {
    stage('Deploy') {
      steps {
        input(message: 'Deploy To', id: 'DEPLOY', ok: 'YES', parameters: [choice(name: 'RELEASE_SCOPE', choices: 'patch\nminor\nmajor', description: 'What is the release scope?')])
      }
    }

  }
}