node {

	stage('SCM'){
		//git clone
		git 'https://github.com/BRAHMAREDDYV/springpetclinic.git'
	}

	stage ('build the package'){
		//mvn package
		sh 'mvn package'
	}
	
	stage ('archival'){
		// archiving artifacts
		archive 'target/*.jar'
	}
	
	stage (' test result'){
		//junit test results
		junit 'target/surefire-reports/*.xml'
	}
}