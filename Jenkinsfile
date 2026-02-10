pipeline {
  
  agent any

  properties([
  parameters([
    [$class: 'SeparatorParameterDefinition', name: '=== DEPLOY OPTIONS ==='],
    string(name: 'ENV', defaultValue: 'dev'),
    booleanParam(name: 'CONFIRM_DEPLOY', defaultValue: false),

    [$class: 'SeparatorParameterDefinition', name: '=== TEST OPTIONS ==='],
    booleanParam(name: 'RUN_TESTS', defaultValue: true)
  ])
])
  
  stages {
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
