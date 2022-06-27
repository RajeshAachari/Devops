groory
   
pipeline{
         
        agent any
           
             stages{
                   stage ('build'){
                          steps{
                              sh 'echo build stage is running  hostname `"hostname"`'
                          }
                        }  


                   stage ('test'){
                       steps{
                           sh 'echo test stage is running'
                       }
                }
            }
}

