job('d_child_Assignment1') {
    scm {
        git {
            branch('main')
            remote {
                url('https://github.com/Rahul-Palande11/SRE-PATH.git')
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
