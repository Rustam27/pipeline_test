pipeline {
    agent {
        label "android"
    }

    stages {
        stage('Hello') {
            steps {
                wrap([$class: 'BuildUser']) {
                    def user = env.BUILD_USER
                    def userFirsName = env.BUILD_USER_FIRST_NAME
                    def userLastName = env.BUILD_USER_LAST_NAME
                    def userId = env.BUILD_USER_ID
                
                    echo 'User: $user'
                    echo 'User firstname: $userFirsName'
                    echo 'User lasttname: $userLastName'
                    echo 'User id: $userId'
                }
            }
        }
    }
}
