pipeline {
    agent any
    stages{
        stage('Build') { 
            steps {
                maven "clean install"
            }
        }
    
        stage("Analisis PMD") {
            steps {
                maven "pmd:pmd"                
            }
        }
        
        stage("Análisis Checkstyle") {
            steps {
                maven "checkstyle:checkstyle" 			
            }
        }
    } 
} 