pipeline {
    agent {
        docker{image 'gcc:latest'}
    }
    stages {
        stage('build') {
            steps {
                sh 'g++ -o my_program Hello.cpp'
            }
        }
    
    stage('Test') {
            steps {
                // Run tests if applicable
                sh './my_program '
            }
        }
}
post {
        success {
            // Add post-build actions if needed
            echo"done success"
        }
        
        failure {
            // Add actions for build failures
            echo"failed"
        }
    }
}
