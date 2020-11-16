pipeline {
    agent any

    environment {
        APP_ID = 'g-java'
    }

    stages {
        stage('Scan from-image') {
            steps {
                echo 'Scanning from-image ...'
                echo 'Getting paths ...'
            }
        }
        stage('Scan current-image') {
            steps {
                echo 'Scanning current-image ...'
                echo 'Getting paths ...'
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