@Library('sharedLibrary') _

pipeline {
    agent any

    stages {
        stage('Demo') {
            steps {
                script {
                    // Call the installNginx function from the shared library
                    sharedLibrary.installNginx()
                }
            }
        }
    }
}
