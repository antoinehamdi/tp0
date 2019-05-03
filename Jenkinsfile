pipeline {
    	agent {
    		label "master"
    }
	options {
		timestamps()
	}
	stages {
		stage('Deploy to test'){
			steps {

        	echo 'Deploying to test'
        	sh 'ansible-playbook -i inventory.ini install_tools.yml'

    }
}
}
}