
pipeline {
    agent { node { label 'LINUX' } } 
    
    stages {
        environment { 
            JAVA_HOME=/opt/jdk1.8.0_121   
        }
        stage('build'){
            steps {
                sh 'ant -f build.xml -v'
            }
        }
    }
}
