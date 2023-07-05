pipeline{
    agent any
    stages {
        stage('Git-Checkout') {
            steps {
                echo "Checking out from Git Repo";
                git branch: 'main', url: 'https://github.com/sagarkalankar1/b_pipeline_github.git'
            }
        }
        
        stage('Build') {
            steps {
                echo "Building the checked-out project";
                sh 'chmod +x Build.sh'
                sh './Build.sh'
            }
        }
        stage('Unit-Test') {
            steps {
                echo "Running the Unit Test";
                sh 'chmod +x Unit.sh'
                sh './Unit.sh'
                /*sh exit ("1");*/
            }
        }
       
        stage('Deploy') {
            steps {
                echo "Deploying to Stage Environment for more tests";
                sh 'chmod +x Deploy.sh'
                sh './Deploy.sh'
            }
        }

    }
}    
