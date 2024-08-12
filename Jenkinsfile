pipeline {
    agent {
        label 'java-agent-slave'
    }
    stages {
        stage ('build') {
            steps {
                echo "this is the stage for mvn app"
                // linux commands
                sh "hostname -i"
            }
        }
        stage ('scriptedstage') {
            steps {
                echo "***********Executing the scripted stage"
                script {
                    def course = "k8s"
                    if (course == "k8s") {
                        println("Thanks for enrolling $course")
                    }
                    else
                        println("do learn k8s")
                }
                sleep 10
            }
        }
        // stage ('sonar') {
        //     steps {
        //         echo "executin sonar stage"
        //     }
        // }
    }
}
