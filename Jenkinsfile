pipeline {
    agent { node { label 'LINUX' } } 
    
    options {
        buildDiscarder(logRotator(numToKeepStr: '2', artifactnumToKeepStr: '1'))
    }
    
    stages {
        stage('build'){
            steps {
                sh 'ant -f build.xml -v'
                  }
                 }
            }
    
    post {
        always {
            archiveArtifacts artifacts: 'dist/*.jar', fingerprint: true
                    
            }
        }
    
}   
