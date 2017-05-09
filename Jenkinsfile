
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
                java -jar '/var/lib/jenkins/workspace/LinuxJobs/Pipeline/dist/rectangle*' 4 5     
            }
    }
}
