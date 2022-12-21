pipeline{
         agent {
                 label{
                      label 'built-in'
                      customWorkspace '/mnt/velocity'
 }
}

               
             stages{
                 stage('deploy httpd'){
                      steps{
                            sh "echo 'test'>>/var/www/html/index.html"
                             sh "sudo chmod -R 777 /var/www/html"
       }
}
                      stage('restart httpd'){
                               steps{
                                      sh "sudo service httpd restart"
                                        
                                        
                               }
  }
}            
}
