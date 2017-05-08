pipeline {
    agent 
    
    stages {
        node('master')
        stage('build'){
            steps {
                sh 'ant -f build.xml -v'
            }
        }
    }
}
