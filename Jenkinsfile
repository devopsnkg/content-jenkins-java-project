pipeline {
    agent { Lable('Linux') }
    
    stages {
        
        stage('build'){
            steps {
                sh 'ant -f build.xml -v'
            }
        }
    }
}
