pipeline{
    agent {label 'ubuntu'}  
    stages{
        stage("build"){
          steps{
            echo 'building...'
            sh '''
            apt install python3.6
            py3 --version
            apt install python3-pip
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
