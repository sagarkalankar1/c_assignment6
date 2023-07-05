pipelineJob('c_child-my-pipeline-job-assgn6') {
    definition {
        cps {
            script('''
                pipeline {
                    agent any
                    stages {
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
