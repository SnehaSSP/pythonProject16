pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                // Checkout the code from the Git repository
                checkout([$class: 'GitSCM', branches: [[name: 'my_latest']], userRemoteConfigs: [[url: 'https://github.com/SnehaSSP/pythonProject16.git']]])
            }
        }
        
        stage('Run Python Scripts') {
            steps {
                // Run the first Python script
                sh 'python ./Mytest_lab.py'
                
                // Run the second Python script
                sh 'python ./lab3.py'

                sh 'python ./mytest_lab1.py'
            }
        }
    }
}
