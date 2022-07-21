pipeline { 
  agent any

  tools{
	nodejs 'Nodejs-18'
  }

  
  stages { 
    stage('clone repository') {
      steps { 
        git 'https://github.com/hellenmawia/gallery.git'
      }
    }
     stage('Build the project') {
      steps { 
        sh 'echo "here we will Build"'
      }
      
    }
    stage('Install Dependencies') {
      steps { 
        sh 'npm install'
      }
    }
    stage('Tests') {
      steps { 
        sh 'npm test'
      }
    }
	stage('Deploy Application') {
      steps {
              sh 'echo "deploy an APP"'
              }
    }
  }
}