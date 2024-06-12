pipeline{
  agent any
  stages{
    stage('deploy to remote'){
      steps{
        sh 'scp -r ${WORKSPACE}/* root@{staging_server}:/home/hamdani'
      }
    }
}

}
