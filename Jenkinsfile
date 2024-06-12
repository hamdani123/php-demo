pipeline{
  agent any
  environment{
    staging_server="103.23.198.160"
  }

  
  stages{
    stage('deploy to remote'){
      steps{
        sh 'scp -r ${WORKSPACE}/* root@${staging_server}:/home/hamdani'
      }
    }
  }
}
