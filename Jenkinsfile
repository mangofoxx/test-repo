pipeline {

     agent any
//   agent { label "jenkins"}

//   parameters {
//     choice(name: 'env', choices: ['staging', 'devbox-core-4', 'preproduction'])
//   }

  options {

    buildDiscarder logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '', daysToKeepStr: '', numToKeepStr: '5')

  }

  stages {

    stage('Hello') {
            steps {
                sh '''
                 mvn clean deploy
                '''
                }
        }

//       steps {
//
//         withCredentials([[$class: 'VaultTokenCredentialBinding', credentialsId: 'vaulttoken', vaultAddr: 'https://localhost:8200']]) {
//
//             }

      }

    }

  }

}