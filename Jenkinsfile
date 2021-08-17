 pipeline {
    agent any
    
    tools {
        terraform 'terraform'
    }
    stages {
        stage ('1 choice') {
           when { 
                              expression {choice == '1'}
                    }
            steps {
                git branch: 'main', credentialsId: 'git-hub', url: 'https://github.com/gowtamdegapudi/aws-jenkins.git'
            }
        }
        stage ("terraform init") {
            steps {
                sh 'terraform init'
            }
        }
        stage ("terraform fmt") {
            steps {
                sh 'terraform fmt'
            }
        }
        stage ("terraform validate") {
            steps {
                sh 'terraform validate'
            }
        }
        stage ("terrafrom plan") {
            steps {
                sh 'terraform plan '
            }
        }
        stage ("terraform apply") {
            steps {
                sh 'terraform apply --auto-approve'
            }
        }
        stage ('2 choice') {
           when {
                             expression { choice == '2' }
                    }
         steps {
                git branch: 'main', credentialsId: 'git-hub', url: 'https://github.com/gowtamdegapudi/aws-jenkins.git'
            }
        }
        stage ("terraform init") {
            steps {
                sh 'terraform init'
            }
        }
        stage ("terraform fmt") {
            steps {
                sh 'terraform fmt'
            }
        }
        stage ("terraform validate") {
            steps {
                sh 'terraform validate'
            }
        }
        stage ("terrafrom plan") {
            steps {
                sh 'terraform plan '
            }
        }
        stage ("terraform apply") {
            steps {
                sh 'terraform apply --auto-approve'
            }
        }
        stage ('3 choice') {
           when {
                             expression { choice == '3' }
           }
          steps {
                git branch: 'main', credentialsId: 'git-hub', url: 'https://github.com/gowtamdegapudi/aws-jenkins.git'
            }
        }
        stage ("terraform init") {
            steps {
                sh 'terraform init'
            }
        }
        stage ("terraform fmt") {
            steps {
                sh 'terraform fmt'
            }
        }
        stage ("terraform validate") {
            steps {
                sh 'terraform validate'
            }
        }
        stage ("terrafrom plan") {
            steps {
                sh 'terraform plan '
            }
        }
        stage ("terraform apply") {
            steps {
                sh 'terraform apply --auto-approve'
            }
        }
    }
}
