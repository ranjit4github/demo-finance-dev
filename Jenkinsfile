@Library('My-Jenkins-SharedLibrary')_

pipeline{
agent any
  stages{
    stage ('Build'){
      steps{
        script{
          build()
        }
      }
    }
    stage ('Upload'){
      steps{
        script{
          nexusUpload()
        }
      }
    }
  }
}
