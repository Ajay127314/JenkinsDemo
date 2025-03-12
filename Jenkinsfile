pipeline {

    agent any
 
    stages {

        stage('Checkout') {

            steps {

                git url: 'https://github.com/Ajay127314/JenkinsDemo.git', branch: 'main'

            }

        }
 
        stage('Build') {

            steps {

                sh 'javac src/com/additiondemo/Addition.java'

            }

        }
 
        stage('Test') {

            steps {

                sh 'java -cp src com.additiondemo.Addition'

            }

        }

    }
 
    post {

        always {

            echo 'Pipeline complete.'

        }

    }

}

 
