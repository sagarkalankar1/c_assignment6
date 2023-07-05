pipelineJob('c_child-my-pipeline-job-assgn6') {
    definition {
        cps {
            script('''
                pipeline {
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
                                // Add build steps here
                                echo 'Building...'
                            }
                        }
                        stage('Test') {
                            steps {
                                // Add test steps here
                                echo 'Testing...'
                            }
                        }
                        stage('Deploy') {
                            steps {
                                // Add deployment steps here
                                echo 'Deploying...'
                            }
                        }
                    }
                }
            ''')
        }
    }
}
