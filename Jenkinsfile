pipeline{
    agent any
    stages{
        stage('Present working Directory'){
            steps{
                sh ' pwd '
            }
        }

        stage('clean working directory'){
            steps{
                sh ' rm -r * '
                sh ' rm -r ../../../../www/html/* '
            }
        }

        stage('copy to html'){
            steps{
                sh ' mv wedding/* ../../../../www/html '
            }
        }
        
       
    }
}