@Library('My-Jenkins-SharedLibrary')_

pipeline{
agent any
  environment{
    demoVar="TestVar"
  }
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
    stage ('Deploy'){
      steps{
        script{
          deployDemo.deploy()
        }
      }
    }
  }
}
