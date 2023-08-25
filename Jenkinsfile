pipeline {
agent {
  label 'slave1-docker'
}

stages{
  stage('testing'){
    agent any 
    steps {
      echo "hello world"
    }
  }

}
post {
  always {
    echo "i am gonna run every single time"
  }
  failure {
    echo "only when something fails"
  }
  success {
    echo "this section will execute when everything is fine"
  }
}

}
