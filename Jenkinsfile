// we use tools selection to auto-install packages or define path of the packages
pipeline {
    agent any
    tools {
        maven 'MAVEN_PATH'
    }
    stages {
        stage ('build') {
            steps {
                sh 'mvn --version'
            }
        }
        stage ('Specificstage'){
            tools {
                jdk 'JDK-17'
            }
            steps {
                echo "***********mvn version with mycustom java at cd /opt"
                sh 'mvn --version'

            }
        }
    }
}
