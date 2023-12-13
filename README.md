pipeline {
 agent any 
 stages {
   stage("clone") {
   steps {
   echo "hello clone welcome to jenkins"
   }
  }
  stage("build") {
    steps {
	echo "hello build welcome to jenkins"
	}
   }
  stege("test") {
    steps {
	echo "hello test welcome to jenkins"
	}
   }
   stage("deploy") {
     steps {
	  echo "hello deploy welcome to jenkins"
	 }
   }
 }
}



