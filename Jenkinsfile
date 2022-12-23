pipeline{
    agent any
    stages{
        stage('Enter into server'){
            steps{
                sh 'ssh -i EC2Server.pem ubuntu@44.204.92.44'
            }
        }
            stage('move to super user'){
                steps{
                sh 'sudo su'
            }
            }
           stage('Back to root directory'){
             steps{
                sh 'cd ../..'
            }
           }
           stage('Install apache2'){
             steps{
                sh 'sudo apt-get insyall apache2 -y'
            }
           }
        stage('clone the project from git lab'){
            steps{
                sh 'git clone https://gitlab.com/dilipkondiboyina2320/mphasis-project.git -b master'
            }
        }
        stage('push to html'){
            steps{
                sh 'cd var/www/html'
            }
        }
        
    }
}