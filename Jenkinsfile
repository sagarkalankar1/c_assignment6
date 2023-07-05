job('c_child_freestyle') {
  scm {
    git {
      remote {
        branch('main')
        url('https://github.com/sagarkalankar1/b_pipeline_github.git')
      }
    }
  }
  steps {
    echo 'Building the checked-out project'
    sh 'chmod +x Build.sh'
    sh './Build.sh'
  }
}
