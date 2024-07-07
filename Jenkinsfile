pipeline {
    agent any
    stages {
        stage ("feature change") {
            when {
                allOf {
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
