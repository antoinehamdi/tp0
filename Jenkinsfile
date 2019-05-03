pipeline {
    	agent {
    		label "vagrant"
    }
	options {
		timestamps()
	}
	stages {
		stage('Deploy to test'){
			steps {

        	echo 'Deploying to test'
        	sh 'ansible-galaxy install -r roles/requirements.yml'
        	sh 'ansible-playbook -i inventory.ini install_tools.yml'

    }
}
}
}