pipeline {
agent any
stages {
  stage('Github-checkin') {
    steps {
      // One or more steps need to be included within the steps block.
	git branch: 'main', credentialsId: 'github-private-key', url: 'git@github.com:Henithvaibav/github-pipeline.git'
    }
  }
  stage('build') {
    steps {
      // One or more steps need to be included within the steps block.
	bat 'Build.bat'
    }
  }

  stage('test') {
    steps {
      // One or more steps need to be included within the steps block.
	bat 'Test.bat'
    }
  }


  stage('quality') {
    steps {
      // One or more steps need to be included within the steps block.
	bat 'Quality.bat'
    }
  }


  stage('deploy') {
    steps {
      // One or more steps need to be included within the steps block.
	bat 'Deploy.bat'
    }
  }
}
}
