pipeline {
    agent any
    stages {
        stage("GitHub Access") {
            steps {
                script {
                    // Clone the GitHub repository
                    git branch: 'main', url: 'https://github.com/Mokshithanaidu/jobs-pipeline.git'
                }
            }
        }
        stage("Java") {
            steps {
                script {
                    // Compile and run Hello.java
                    bat '''
                    javac hello.java
                    java hello
                    '''
                }
            }
        }
        stage("Python") {
            steps {
                script {
                    // Run hello.py
                    python 'hello.py'
                }
            }
        }
    }
}
