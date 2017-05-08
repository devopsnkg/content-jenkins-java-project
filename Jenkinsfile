pipeline {
    
    node('Linux')
    
    stages {
        stage('build'){
            steps {
                sh 'ant -f build.xml -v'
            }
        }
    }
}
