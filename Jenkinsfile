pipeline {
    agent node('master')
    
    stages {
        
        stage('build'){
            steps {
                sh 'ant -f build.xml -v'
            }
        }
    }
}
