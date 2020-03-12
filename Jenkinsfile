pipline {
    angent any
    stages {
        stage ('Build') {
            steps {
                echo "Running build automation"
                // the next command is used for developing purposes as it speeds up the code, it's local instruction to Jenkins itself
                sh './gradlew build --no-daemon'
                // the command bellow stores the artifacts 
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
    }
}