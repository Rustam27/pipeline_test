pipeline {
    agent {
        label "android"
    }
    
    environment {
        wrap([$class: 'BuildUser']) {
            USER_ID = env.BUILD_USER_ID
        }
    }

    stages {
        stage('Hello') {
            steps {
                echo "${USER_ID}"
            }
        }
    }
}
