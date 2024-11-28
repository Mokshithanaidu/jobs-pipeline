pipeline {
    agent any
    stages {
        stage("GitHub Access") {
            steps {
                script {
                    // Clone the GitHub repository
                    git branch: 'main', url: 'https://github.com/<your-username>/<your-repository>.git'
                }
            }
        }
        stage("Java") {
            steps {
                script {
                    // Compile and run Hello.java
                    bat '''
                    javac Hello.java
                    java Hello
                    '''
                }
            }
        }
        stage("Python") {
            steps {
                script {
                    // Run hello.py
                    python3 'hello.py'
                }
            }
        }
    }
}
