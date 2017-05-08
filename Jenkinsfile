pipeline {
    agent ['Python']
    
    stages {
        
        stage('build'){
            steps {
                sh 'ant -f build.xml -v'
            }
        }
    }
}
