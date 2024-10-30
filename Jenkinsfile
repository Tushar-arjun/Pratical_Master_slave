pipeline{
	    agent{
	        label {
	            label "job2"
	            
	        }
	    }
	    stages{
	        stage("install httpd"){
	            steps{
	                sh '''
	            sudo yum install httpd -y
	            sudo systemctl start http
	            '''
	            }
	
	        }
	         stage("deploy httpd"){
	            steps{
	                sh '''
	                sudo chmod -R 777 /var/www/html
	                echo "This is Branch -2 Test web appliation" > /var/www/html/index.html
	                '''
	            }
	         }            
	
	        
	           
	            
	    }
	      	        
	}
