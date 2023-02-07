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
              mpirun -np 2 python3 mpi.py
             '''
           }
        }  
      }
}
