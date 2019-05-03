pipeline {
  agent any

  stages {
    stage("One") {
      steps {
        echo "Hello"
      }
    }
   stage("Evaluate Master") {
      when {
	branch "master"
      }
      steps {
        echo "Hello Master!!"
      }
    }
     stage ("Evaluate Dev"){

      when{
	branch "Dev"
	}
	steps {
	  echo "Hello Dev!!"
	}
      }
      stage ("Evaluate Test"){
	when{
	  branch "Test"
	}
	steps{
	   echo "Hello Test!!"
	}
    }
  }
}
