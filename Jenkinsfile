pipeline {
    agent any

    stages {
        stage('git repo & clean') {
            steps {
                bat "git clone https://github.com/piyushbodhani1/Devops_Product.git"
                bat "mvn clean -f Devops_Product"
            }
        }
         stage('install') {
            steps {
                bat "mvn install -f Devops_Product"
            }
        }
        stage('test') {
            steps {
                 bat "mvn test -f Devops_Product"
            }
        }
    }
}
