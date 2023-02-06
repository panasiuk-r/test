pipeline{
    agent {
        docker { image 'node:16-alpine' }
    }  
    stages{
        stage("build"){
          steps{
            echo 'building...'
            sh '''
            node --version
            // py3 --version
            // python3 -m pip install mpi4py
            '''
          }
        }
        stage("test"){
           steps{
              echo 'testing...'
             sh '''
              // mpirun -np 4 python3 mpi.py
             '''
           }
        }  
      }
}
