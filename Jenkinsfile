pipeline {
   agent {label 'DOCKER'}
   stages {
     stage('vcs') {
       steps { 
    git url: 'https://github.com/Azure-Samples/js-e2e-express-server.git', 
    branch: main
       }
     }
       stage('build') {
     steps(
        sh """
         npm install
         npm start
         """

     )
       }

     }
   }
