pipeline {
	agent {
		label {
			label "qa"
			customWorkspace "/mnt/avi"
		}
	}
			stages {
				stage ("stage-1"){
					steps {
					
						git "https://github.com/awantika-kamble/project.git"
					}
				
				}
				stage ("stage-2"){
					steps {
					sh "yum install httpd -y"
					sh "service httpd start"
					sh "cp /mnt/avi/index.html /var/www/html"
					sh "service httpd restart"
					
					}
				}
					
			
			}
}
