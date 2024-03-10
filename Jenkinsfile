pipeline
{
  agent any
  stages
  {

    stage('Build')
    {
      steps
      {
        build 'PES2UG21CS027-1'
        sh 'g++ L.cpp -o output'
      }
    }

    stage('Test')
    {
      steps
      {
        sh './output'
      }
    }
    stage('Deploy')
    {
      steps
      {
        echo 'deploy'
      }
    }
  }

  post
  {
    failure
    {
      error 'Pipeline failed'
    }
  }
}
    
        

    
        
