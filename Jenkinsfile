pipeline 123{
  agent any
  environment{
    staging_server="103.117.57.55"
  }
  stages{
    stage('deploy to remote'){
      steps{
        withCredentials([sshUserPrivateKey(credentialsId: 'agent-aplikasi', keyFileVariable: '', usernameVariable: 'aplikasi')]) {
    // some block
      }
        sh 'scp ${WORKSPACE}/* aplikasi@${staging_server}:/home/aplikasi/php-demo/'
      }
    }
  }
}
  
