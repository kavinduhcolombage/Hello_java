pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                echo "Cloning the GitHub repository..."
                git branch: 'main', url: 'https://github.com/kavinduhcolombage/Hello_java.git'
            }
        }

        stage('Compile Java Code') {
            steps {
                echo "Compiling the Java file..."
                sh 'javac HelloWorld.java'
            }
        }

        stage('Run Java Program') {
            steps {
                echo "Running the Java program..."
                sh 'java HelloWorld'
            }
        }
    }
}
