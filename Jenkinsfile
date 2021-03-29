pipeline {
    agent any
    stages{
        stage('Build') { 
            steps {
                bat "mvn clean install"
            }
        }
    
        stage("Analisis PMD") {
            steps {
                bat "mvn pmd:pmd"                
            }
        }
        
        stage("Análisis Checkstyle") {
            steps {
                bat "mvn checkstyle:checkstyle" 			
            }
        }
    } 
} 