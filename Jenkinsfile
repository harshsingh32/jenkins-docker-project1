pipeline {

    agent {

        docker {

            image 'my-project'

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
 
