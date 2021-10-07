pipeline {
    agent any 
    stages{
        stage('Build') {
            steps {
                echo 'Running build automation'
                sh './gradelw build --no-deamon'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
    }
}
