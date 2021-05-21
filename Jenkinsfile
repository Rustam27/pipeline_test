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
                        USER_FIRST_NAME = env.BUILD_USER_FIRST_NAME
                        USER_LAST_NAME = env.BUILD_USER_LAST_NAME
                        USER_USER = env.BUILD_USER
                    }   
                    
                    echo "${USER_ID}"
                    echo "${USER_FIRST_NAME}"
                    echo "${USER_LAST_NAME}"
                    echo "${USER_USER}"
                }
            }
        }
    }
}
