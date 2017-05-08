
pipeline {
    agent { node { label 'LINUX' } } 
    
    stages {
        
        stage('build'){
            steps {
                sh 'ant -f build.xml -v'
            }
        }
    }
}
