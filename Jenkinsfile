pipelineJob('Clone Repository') {
  definition {
    cps {
      script("""
        node {
          stage('Clone Repository') {
            git branch: 'main', url: 'https://github.com/sagarkalankar1/b_pipeline_github.git
            echo "Created sagar beta"
          }
        }
      """)
    }
  }
}
