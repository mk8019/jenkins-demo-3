pipeline{
  agent any
  
  environment{
      Release = '20.04'
  }
  
  stages{
    stage('build'){
      agent any
      environment{
        LOG_LEVEL='INFO'
      }
      steps{
        echo "Building release ${Release} with log level ${LOG_LEVEL}..."
      }
    }
    stage('Test'){
      steps{
        "Testing. I cna see the release ${Release} but not the log level ${LOG_LEVEL}"
      }
    }
    
  }
  
}
