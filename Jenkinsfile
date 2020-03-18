pipeline {
        agent any
        stages {
                   stage('Upload to AWS')  {
                        steps {
                                  withAWS(region:'us-west-2',credentials:'AWS-Static')
                                {
                                   s3Upload(file:'index.html', bucket:'kalpeshudacityp4')
                                 }
                         }
                               }
                }
          }
