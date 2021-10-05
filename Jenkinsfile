pipeline {
    agent { 
      docker {
          image 'alpine:latest'
          reuseNode true
      }
      }
    stages {
        stage('Example') {
            steps {
                echo 'Hello World. This is wonderful world'

                script {
                    def browsers = ['chrome', 'firefox', 'safari', 'vimium']
                    for (int i = 0; i < browsers.size(); ++i) {
                        echo "Testing the ${browsers[i]} browser"
                    }
                }
            }
        }
    }
}

