job('d_child_Assignment1') {
    scm {
        git {
            branch('main')
            remote {
                url('https://github.com/sagarkalankar1/c_Assignment6_jobfile.git')
            }
        }
    }

    steps {
        shell '''
            javac Hello.java
            java Hello
        '''
    }
}
