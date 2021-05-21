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
                    }   
                    
                    echo "${USER_ID}"
                }
            }
        }
    }
}
