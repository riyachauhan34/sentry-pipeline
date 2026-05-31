@Library('ansible-lib') _

pipeline {

    agent any

    stages {

        stage('Load Config') {

            steps {

                script {

                    config = load 'config.groovy'

                }

            }

        }

        stage('Run Shared Library') {

            steps {

                script {

                    deploySentry(config)

                }

            }

        }

    }

}
