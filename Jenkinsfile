pipeline {
  agent any

  stages {
    stage("One") {
      steps {
        echo "Hello"
      }
    }
    stage("Evaluate branches") {
      when {
	branch "master"
      }
      steps {
        echo "World"
        echo "Heal it"
      }

      when{
	branch "Dev"
	}
	steps {
	  echo "Hello Dev!!"
	}
	when{
	  branch "Test"
	}
	steps{
	   echo "Hello Test!!"
	}
    }
  }
}
