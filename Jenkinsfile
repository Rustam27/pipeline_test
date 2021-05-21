pipeline {
    agent {
        label "android"
    }
    
    stages {
        stage('Hello') {
            steps {
                script {
                    wrap([$class: 'BuildUser']) {
                        USER_ID = env.BUILD_USER_ID
                        USER_USER = env.BUILD_USER
                    }   
                    
                    echo "${USER_ID}"
                    echo "${USER_USER}"
                }
            }
        }
    }
}
