pipeline {
    agent {
        label 'master'
          }

    stages {
        stage('Init'){
            agent {
                    label 'master'
                  }
        	steps{
        		    script{		
         
		     sh 'echo $GIT_BRANCH > branch.txt '
             sh 'cat branch.txt | cut -b 8- > branch.txt'
              sh 'cat branch.txt | cut -d "." -f 1'
           
		     sh'rm branch.txt'
                 
                
				        }
			      }
            }
    }
}
