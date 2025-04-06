pipeline {
  agent any
  stages {
    stage('Build_Stage') {
      steps {
        echo 'Build Is Done '
      }
    }

    stage('Test_Stage') {
      parallel {
        stage('Test1') {
          steps {
            echo 'Test_1'
          }
        }

        stage('Test_1') {
          steps {
            echo 'Test_2 Runned'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Code_deployed'
      }
    }

  }
}