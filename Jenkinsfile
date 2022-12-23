pipeline{
    agent any
    stages{
        
           
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