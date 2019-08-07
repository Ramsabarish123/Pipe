pipeline{
  stages{
  
  steps{
      try {
							sh """
								mkdir $(JOB_NAME).env
								echo $(Source_TD_Name) >> $(JOB_NAME).env
								echo $(Target_TD_Name) >> $(JOB_NAME).env
								echo $(DSC_Host_Name) >> $(JOB_NAME).env
								echo $(Docker_Host_Name) >> $(JOB_NAME).env
								
                               """
                        } catch(error) {
                            echo 'Test failed'
                            throw error
                        }
  
  }
  
  }
    
}
