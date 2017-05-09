
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
                relativeTargetDir('/var/lib/jenkins/workspace/LinuxJobs/Pipeline/dist/')
                sh 'java -jar rectangle* 4 5'     
            }
        }
    }
}
