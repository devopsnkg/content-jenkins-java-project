pipeline {
    agent { node { label 'Linux' } } 
    
    stages {
        
        stage('build'){
            steps {
                sh 'ant -f build.xml -v'
            }
        }
    }
}
