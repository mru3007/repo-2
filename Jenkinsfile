pipeline{
  agent any {
    stages {
      stage ("start httpd"){
                  steps {
                         sh " sudo systemctl start httpd"
                  }
      }
      stage ("clear workspace"){
                  steps {
                         sh "rm -rf /var/www/html/*"
                  }
      }
      stage ("deploy webpage"){
                  steps {
                          sh "sudo echo 'this is pipeline deployment' >> /var/www/html/index.html"
                          sh "sudo chmod -R 777 /var/www/html/index.html"
                  }
      }
      
    }
    
  
  }

}
