pipeline {
    agent any
    stages {
        stage ('Refresh instance ') {
            steps {
                sh 'aws autoscaling start-instance-refresh \
                      --auto-scaling-group-name terraform-autoscaling   \
                      --preferences '{"InstanceWarmup": 400, "MinHealthyPercentage": 50}'
'

             }
         }
      }
  }
