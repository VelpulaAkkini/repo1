pipeline {
   agent any
     stages {
	  stage ("test") {
	   steps {
	     echo "hello test welcome to my new pipeline"
	   }
	  
	  }
	 }

}
