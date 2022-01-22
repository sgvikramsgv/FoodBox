pipeline
{
  agent any
  stages
  {
    stage('Build')
    {
      steps
      {
        echo 'Build app'
      }
    }
    stage ('Test')
    {
     steps
      {
      echo 'Test App'
      }
    }
    stage ('Deploy')
    {
      steps
      {
        echo 'Deploy App'
      }
    }
  }
  post
  {
    always
    {
    emailext body: 'Summary: Pipeline Build Successful for FoodBox Application', subject: 'Pipeline Status', to: 'deebikaece@gmail.com'
    }
  }
}
