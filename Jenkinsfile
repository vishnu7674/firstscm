pipeline {
    agent any 
    stages {
        stage ('build') {
            steps {
                echo "*********Entering build block*******"
                retry(3) {
                    echo "welcome to d4"
                    error "testing the retry block"
                }
                echo "***********after 3 retrys*****"
            }
        }
    }
}
