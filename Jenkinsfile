pipeline {
    agent {
        label 'master'
          }

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
                echo " $version"
                echo "$subversion"
            }
        }
    }
}
