pipeline {
    agent any


    stages {
        stage('Clone Repo') {
            steps {
                // Get some code from a GitHub repository
                git branch: 'main', url: 'https://github.com/yoyoraso/Jenkins-demo.git'
                sh "ls"
               
            }
        }
        stage('Rename and Archive') {
            steps {
                sh 'mv test.txt Muhammad_Osama.txt'
            }
        }
        
    }
    post {
        success {
            sh 'echo "Hello from Muhammad" >> Muhammad_Osama.txt' 
            archiveArtifacts artifacts: 'Muhammad_Osama.txt', onlyIfSuccessful: false
        }

    }
}
