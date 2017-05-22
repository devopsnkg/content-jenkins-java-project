
pipeline {
    agent { node { label 'LINUX' } } 
    
    stages {
        stage('build'){
            steps {
                sh 'ant -f build.xml -v'
                  }
                 }
            }
    POST {
        always {
            archive 'dist/*.jar'
                    
            }
        }
    }
}   
