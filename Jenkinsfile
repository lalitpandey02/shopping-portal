pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'this is the build job'
        sh 'npm install'
      }
    }

    stage('test') {
      steps {
        echo 'this is the test job'
        sh 'npm test'
      }
    }

    stage('package') {
      steps {
        echo 'this is the package job'
        sh 'npm run package'
      }
    }

<<<<<<< HEAD
    stage('artifact') {
=======
    stage('archive') {
>>>>>>> bcb7dc928025baf3814556ca4715166c13ff0ed4
      steps {
        archiveArtifacts '**/distribution/*.zip'
      }
    }

  }
  tools {
    nodejs 'nodejs'
  }
  post {
    always {
      echo 'this pipeline has completed...'
    }

  }
<<<<<<< HEAD
}
=======
}
>>>>>>> bcb7dc928025baf3814556ca4715166c13ff0ed4
