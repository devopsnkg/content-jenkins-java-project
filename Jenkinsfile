pipeline {
    agent { node { label 'LINUX' } } 
    
    options {
        buildDiscarder(logRotator(numToKeepStr: '20', artifactNumToKeepStr: '10'))
    }
    
    stages {
        stage('Unit Test'){
            steps {
                sh 'ant -f test.xml -v'
                junit 'reports/report.xml'
            }
        }
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
