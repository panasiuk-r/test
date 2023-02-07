pipeline{
    agent {label 'python'}  
    stages{
        stage("build"){
          steps{
            echo 'building...'
            sh '''
            python3 --version
            '''
          }
        }
        stage("test"){
           steps{
              echo 'testing...'
             sh '''
              mpirun -np 1 python3 mpi.py
             '''
           }
        }  
      }
}
