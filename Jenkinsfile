pipeline{
  agent any 
  
  stages{
    stage("build"){
      steps{
        echo 'building...'
        sh '''
        pip install -r requirments.txt
        
        '''
      }
      stage("test"){
        steps{
           echo 'testing...'
          sh '''
          python3 hello.py
          '''
        }
      }
    }
  }
}
