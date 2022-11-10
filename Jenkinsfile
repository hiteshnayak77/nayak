currentBuild.displayName = "Final_Demo # "+currentBuild.number

   def getDockerTag(){
        def tag = sh script: 'git rev-parse HEAD', returnStdout: true
        return tag
        }
        

pipeline{
        agent any  
        environment{
	    Docker_tag = getDockerTag()
        }
        
        stages{

              stage('build')
                {
              steps{
                  script{
		            echo "$Docker_tag"
			
                       }
                    }
                 }
		 
	
		
               }
	       
	       
	       
	      
    
}
