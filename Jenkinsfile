pipeline{
  agent any
  stages{
    stage("build"){
      steps{
        echo 'building...'
        sh '''
         python -m pip install mpi4py
        '''
      }
    }
    stage("test"){
       steps{
          echo 'testing...'
         sh '''
           mpirun -np 4 python mpi.py
         '''
       }
    }  
  }
}
