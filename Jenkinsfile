pipeline{
agent any
stages{
stage('git checkout'){
  when {
    branch 'dev'
  }
  steps{
    echo 'This is dev stage'
  }
}
  stage('Maven'){
  when {
    branch 'prod'
  }
  steps{
    echo 'This is prod stage'
  }
}
  stage('SonarQube'){
  when {
    branch 'uat'
  }
  steps{
    echo 'This is uat stage'
  }
}
  stage('Nexus'){
  when {
    branch 'deploy'
  }
  steps{
    echo 'This is deploy stage'
  }
}
}
}
