pipeline{
    agent {
        docker { image 'python:3' }
    }  
    stages{
        stage("build"){
          steps{
            echo 'building...'
            sh '''
             py3 --version
             python3 -m pip install mpi4py
            '''
          }
        }
        stage("test"){
           steps{
              echo 'testing...'
             sh '''
               mpirun -np 4 python3 mpi.py
             '''
           }
        }  
      }
}
