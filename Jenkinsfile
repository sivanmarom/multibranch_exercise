pipeline {
	agent any
	stages{
		stage("README search"){
			steps{
				sh '''if [ -f README.md ]; then echo README.md ; fi echo "The name of this branch is : main branch"
'''				
				script{
				def file_content =readFile(file: "README.md")
				mail bcc: '', body: 'file_content', cc: '', from: '', replyTo: '', subject: 'README.md content', to: 'sivmarom@gmail.com'
}
}
}
}
}
