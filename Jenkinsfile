pipeline {
    agent any

    environment {
        APP_ID = 'g-java'
    }

    stages {
        stage('Starting Clair scanner ...') {
            steps {
                sh 'docker run -p 5432:5432 -d --name clair-db arminc/clair-db:latest'
                sh 'docker run -p 6060:6060 --link clair-db:postgres -d --name clair arminc/clair-local-scan:latest'
            }
        }
        stage('Scan from-image') {
            steps {
                echo 'Scanning from-image ... (Clair and IQ CLI)'
                
                echo 'Getting paths ... (custom script)'
            }
        }
        stage('Scan current-image') {
            steps {
                echo 'Scanning current-image ... (Clair and IQ CLI)'
                echo 'Getting paths ... (custom script)'
            }
        }
        stage('Compare and separate reports') {
            steps {
                echo 'Comparing reports ...'
            }
        }
        stage('Output') {
            steps {
                echo 'Link to from-image IQ report: XXXXX'
                echo 'Link to from-image path report: XXXXX'
                echo 'Link to current-image IQ report: XXXXX'
                echo 'Link to current-image path report: XXXXX'
            }
        }
        
    }
}