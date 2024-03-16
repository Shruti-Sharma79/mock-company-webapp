pipeline {
  /*
   * TODO: Implement pipeline stages/steps
   *   See documentation: https://www.jenkins.io/doc/book/pipeline/syntax/#stages
   */
   pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                // Build stage - Compiles the code
                script {
                    echo 'Building the project...'
                    sh './gradlew assemble'
                }
            }
        }
        stage('Test') {
            steps {
                // Test stage - Runs the tests
                script {
                    echo 'Running tests...'
                    sh './gradlew test'
                }
            }
        }
    }
}

}
