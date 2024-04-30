pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                // Checkout the code from the Git repository
                git branch: 'my_latest', url: 'https://github.com/SnehaSSP/pythonProject16.git'
            }
        }
        
        stage('Run Python Scripts') {
            steps {
                // Run the first Python script
                sh 'lab3.py'
                
                // Run the second Python script
                sh 'mytest_lab.py'

                sh 'mytestlab1.py'
            }
        }
    }
}
