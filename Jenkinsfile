
pipeline {
    agent { node { label 'LINUX' } } 
    
    stages {
        stage('build'){
            steps {
                sh 'ant -f build.xml -v'
                  }
                 }
        stage('Test') {
            steps {
                java -jar '/var/lib/jenkins/workspace/Linux\ Jobs/Pipeline/dist/rectangle_${env.MAJOR_VERSION}.42.jar' 4 5     
            }
    }
}
