pipeline{
  agent any
  stages{
    stage("build"){
      steps{
        echo 'building...'
        sh '''
        '''
      }
    }
    stage("test"){
       steps{
          echo 'testing...'
         sh '''
          mpiexec -n 4 python3 mpi.py
         '''
       }
    }  
  }
}
