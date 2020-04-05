pipeline {
  agent any
  stages {
    stage('Upload to AWS') {
      withAWS(region:'us-east-2') {
          s3Upload(file:'index.html', bucket:'wangzuowen-static', path:'./')
      }  
    }
  }
}
