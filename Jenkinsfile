pipeline {

    tools{

        maven 'mvn'

        jdk 'jdk'

    }

    agent any

 

    stages {

        stage('checkout') {

            steps {

                git 'https://github.com/samiksha0700/DevOpsClassCodes.git'

            }

        }

        stage('pipeline1'){

            steps{

                sh 'mvn compile'

            }

        }

        stage('test'){

            steps{

                sh 'mvn test'

            }

        }

        stage('code coverage'){

            steps{

                sh 'mvn pmd:pmd'

            }

        }

        stage('package'){

            steps{

                sh 'mvn package'

            }

        }

    }

}
