pipeline {
    agent any
    parameters {
        booleanParam(name: "TEST_BOOLEAN", defaultValue: true, description: "Sample boolean parameter")
        string(name: "TEST_STRING", defaultValue: "Jenkins", trim: true, description: "Sample string parameter")
        choice(name: "TEST_CHOICE", choices: ["Dev", "Uat", "Prod"], description: "Sample multi-choice parameter")
    }
    stages {
        stage("Build") {
            steps {
                echo "Build stage."
                echo "Hello $params.TEST_STRING"
            }
        }
        stage("Test") {
            steps {
                echo "Test stage."
            }
        }
        stage("Release") {
            steps {
                echo "Release stage."
            }
        }
    }
}
