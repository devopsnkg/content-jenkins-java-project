
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
                cd '/var/lib/jenkins/workspace/LinuxJobs/Pipeline/dist/'
                java -jar 'rectangle*' 4 5     
            }
    }
}
