pipeline {
    agent any // Allocate an agent for the pipeline to run on



    stages {
        stage('Build') { // Stage for building the project
            steps {
                sh './gradlew build' // Execute the Gradle build task using the Gradle Wrapper
            }
        }

        stage('Run') { // Stage for running/testing the built project
            steps {
                // Example: Running a specific Gradle task like 'test' or 'run'
                // sh './gradlew test' // Execute the Gradle test task
                // Or to run the application if it's a runnable project:
                sh './gradlew run'
            }
        }
    }
}
