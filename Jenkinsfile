pipeline {
     agent {
	     
		 label "built-in"
	 
	 }
	 
	 stages {
	     
		 stage ('Install-HTTPD') {
		 
		 steps {
		    
		    sh "yum install httpd -y"
            sh "service httpd start"
            sh "echo 'Hello All' >> /var/www/html/index.html"
            sh "chmod -R 777 /var/www/html/index.html"
		}
	   }
	 }
}
