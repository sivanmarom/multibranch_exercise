pipeline {
	agent any
	stages {
		stage('README.md search') {
			steps {
				sh '''
					if [ -f README.md ]; then echo README.md ; fi
					echo "The name of this branch is : $BRANCH_NAME"
				'''
				script {
					def file_content = readFile(file: "README.md")
					mail to: "mail.sivmarom@gmail.com", subject: "README content", body: file_content
				}
			}		
		}	
	}
}

