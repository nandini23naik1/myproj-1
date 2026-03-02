pipeline {
    agent any

    stages {
        stage('fetch file') {
            steps {
            git' https://github.com/nandini23naik1/myproj-1.git'
            }
        }
         stage('building') {
            steps {
                echo 'building project......'
               
            }
        }
        stage('Executing') {
            steps {
                echo 'Executing  progress......'
                 bat 'python test.py'
            }
        }
        stage('deploy') {
            steps {
                echo 'deploying......'
                
            }
        }
    }
    post{
     success{
         echo"pipeline executed succesfully"
     }
failure{
    echo"pipeline failed"
    
}
}
     }
     
    
