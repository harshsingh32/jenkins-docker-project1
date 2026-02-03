pipeline {

    agent {

        docker {

            image 'my-project'
            args '-u root'

        }

    }


    stages {
        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/harshsingh32/jenkins-docker-project1.git'
            }
        }


    stages {

        stage('Build') {

            steps {

                echo "Inside Docker container"

                sh 'ls -l /app'

            }

        }

        stage('Run Script') {

            steps {

                sh './script.sh'

            }

        }

        stage('Test HTML') {

            steps {

                sh 'cat index.html'

            }

        }

    }

}
 
