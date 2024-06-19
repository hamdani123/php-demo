pipeline {
  agent any
  environment {
    staging_server="103.117.57.55"
    remote_dir="/home/aplikasi/rolebase"
    remote_user="aplikasi"
  }
  stages {
    stage('Deploy') {
      steps {
        sh 'scp -r ${WORKSPACE} ${remote_user}@${staging_server}:${remote_dir}'
      }
    }
  }
}
