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
                                echo "Building the checked-out project";
                                sh 'chmod +x Build.sh'
                                sh './Build.sh'
                            }
                        }
                    }
                }
            ''')
        }
    }
}
