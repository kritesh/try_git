pipeline {
    agent any 
    stages {
        stage('one') {
            steps {
                echo 'hi'
            }
        }
       stage('two') {
           steps {
                  input('Do you want to procced?')
           }
        }

       stage('three') {
             when {
                   not {
                       branch "master"
                   }
             }        
           steps {
                  echo "Hello"
           }   
        }


     stage('four') {
                    parallel {
                         stage('Unit test') {
                              steps {
                                    sleep 20
                                    }     
     }

                         stage('parallel ste') {
                              steps {
                                    echo 'This is parallel step'
}
                                    
                              }
}
}


    }
}
