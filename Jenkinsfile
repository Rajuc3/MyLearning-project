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
}
