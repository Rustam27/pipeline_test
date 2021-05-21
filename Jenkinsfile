pipeline {
    agent {
        label "android"
    }

    stages {
        stage('Hello') {
            steps {
                script {
                    wrap([$class: 'BuildUser']) {
                        def user = env.BUILD_USER_ID
                        echo "$user"
                    }   
                }
            }
        }
    }
}
