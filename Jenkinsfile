@Library('sharedlibraries@master')
// import os_directoryMake
// import git_checkoutBranch
// import listFiles
import go_setEnv

pipeline {
  agent any
  environment {
//    OUT_DIR = "${env.WORKSPACE}/out"
    IN_DIR = "in"
    OUT_DIR = "out"
  }
  tools { 
    maven 'maven-3.6.1' 
  }
  stages {
/*    stage('Checkout') {
        steps {
          git_checkoutBranch(
                    branch: 'refs/heads/master',
                    relTargetDir: 'src/data-collection',
                    url: 'mvn_SHconstruction.git'
          )
        }
    }
    stage('List files') {
      steps {
        listFiles ("-a")
      }
    }

    stage ('creating a directory') {
      steps {
        echo "Creating a directory"
        os_directoryMake ("${OUT_DIR}")
      }
    }
  }

    stage('compile all modules') {
      steps {
        cleanWs()
     //   sh label: 'message from Jenkinsfile',
     //           script: '${os_directoryMake(testDir)}'

       os_directoryMake("Create a directory", "${OUT_DIR}/${IN_DIR}")

     //   sh label: 'message from Jenkinsfile',
     //           def dirCreate = os_directoryMake ("${OUT_DIR}")
     //           script: '$dirCreate'
      }
    }
  }
*/
    stage('List files') {
      steps {
        go_setEnv ('a':"${IN_DIR}",'b':"${OUT_DIR}",'c':3)
      }
    }
  }
}
// def map = ['a':"${IN_DIR}", 'b':"${OUT_DIR}", 'c':3]
