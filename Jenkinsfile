pipeline {
    agent any
    
    environment {
        API_KEY = credentials('todo-app/api-key')
    }
    
    stages {
        stage('Test API Key') {
            steps {
                // The actual value will be masked in logs
                echo "Using API Key: ${API_KEY}"
                
                // If you're using bash/shell
                sh '''
                    echo "Testing API Key presence..."
                    if [ -n "$API_KEY" ]; then
                        echo "API Key is set"
                    else
                        echo "API Key is not set"
                    fi
                '''
                
                // You could also test your API connection here
                // sh 'curl -H "Authorization: Bearer $API_KEY" https://api.example.com'
            }
        }
    }
}
