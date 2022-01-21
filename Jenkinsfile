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
	echo "build successfully"
    }
  }

  stage('test') {
    steps {
      // One or more steps need to be included within the steps block.
	echo "Test successful"
    }
  }


  stage('quality') {
    steps {
      // One or more steps need to be included within the steps block.
	echo "Quality successful"
    }
  }


  stage('deploy') {
    steps {
      // One or more steps need to be included within the steps block.
	echo "deply successful"
    }
  }
}
}
