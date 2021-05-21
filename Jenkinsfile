pipeline {
    agent {
        label "android"
    }
    
    environment {
        BUILD_USER = "${env.BUILD_USER}"
    }

    stages {
        stage('Hello') {
            steps {
                echo BUILD_USER
            }
        }
    }
}
