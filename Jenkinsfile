pipeline {
  
  agent any

  parameters {
        string(name: 'ENV', defaultValue: 'dev', description: 'Target environment')
        booleanParam(name: 'RUN_TESTS', defaultValue: true, description: 'Run tests?')
        choice(name: 'REGION', choices: ['us-east-1', 'eu-west-1'], description: 'AWS region')
    }
  
  stages {

    parallel(
    stage("build") {
      steps {
        echo 'Building the application'
        echo 'Hali'
      } 
    }

stage("test") {
      steps {
        echo 'Testing the application'
      } 
    }

stage("deploy") {
      steps {
        echo 'Deploying the application'
      } 
    }
  }
}
