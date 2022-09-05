pipeline {
      agent any
      stages {
            stage('Dev') {
                  steps {
                        echo 'Hi, this is Anshul from LevelUp360'
                        echo 'We are Starting the Testing'
                  }
            }
            stage('Build') {
                  steps {
                        echo 'Building Sample Maven Project'
                  }
            }
            stage('Test') {
                  steps {
                        echo "Deploying in Staging Area"
                  }
            }
            stage('Deploy to prod') {
                  steps {
                        echo "Deploying in Production Area"
                  }
            }
      }
}
