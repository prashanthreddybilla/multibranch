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
             sh 'cat branch.txt | cut -b 8- > br.txt'
              sh 'cat br.txt | cut -d "." -f 1'
           
		     sh'rm branch.txt'
				    sh 'rm br.txt'
                 
                
				        }
			      }
            }
    }
}
