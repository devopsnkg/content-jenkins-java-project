export JAVA_HOME=/opt/jdk1.8.0_121
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
