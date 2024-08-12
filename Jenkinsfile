pipeline {
    agent any
    stages {
        stage ('timeout') {
            steps {
                timeout(time: 5, unit: 'SECONDS') {
                    echo "sleeping for 60secs"
                    sleep 60

                }
            }
        }
    }
}
