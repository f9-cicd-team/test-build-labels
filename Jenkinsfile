pipeline {
    agent none
    
    options {
        timeout(15)
    }
    
    stages {
        stage('test base label') {
            agent {
                label "base"
            }
            steps {
                echo "hello from base agent"
            }
        }
        stage('test generic label') {
            agent {
                label "base"
            }
            steps {
                echo "hello from generic agent"
                sh 'pip3 --version'
                sh 'python3 -V'
            }
        }
    }
}
