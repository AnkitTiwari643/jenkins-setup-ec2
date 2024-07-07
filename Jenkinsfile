pipeline {
    agent any
    stages {
        stage ("feature change") {
            when {
                allof {
                    changeRequest()
                }
            }
            steps {
                sh "echo testing feature"
            }
        }
        stage ("transform change") {
            steps {
                sh "echo testing transform"
            }
        }
    }
}
