pipeline {
  agent any
  stages {
    stage('Upload to AWS.') {
      parallel {
        stage('Upload to AWS.') {
          steps {
            sh 'echo "Hello World"'
            sh '''
             echo "Multiline shell steps works too"
             ls -lah
         '''
          }
        }

        stage('DeployingProject3') {
          steps {
            s3Upload 'amanuelbucketproject3'
          }
        }

      }
    }

  }
}