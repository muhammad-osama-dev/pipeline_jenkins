@Library('sharedLibrary')_
    stage('Demo') {
        installnginx
        echo 'here'
    stage('Another Stage') {
        agent { label 'agent1' } // Specify the worker node where you want to run this stage
        steps {
            // Define the steps or tasks you want to perform on the worker node here
            // For example, you can run shell commands, execute scripts, or call shared library functions.
            sh 'echo "This is another stage"'
            // Add more steps as needed.
    }
    }    
}
