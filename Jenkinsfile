node {

    stage "Checout HRMS Test Collection"
    // Checkout
    git branch: ‘master’,url: ‘https://github.com/toolsqacn/PostmanFullStackChat&#8217;

    stage "Run CRMS API Test"
        sh "newman run epmployee.postman_collection.json --reporters cli,html --reporter-html-export ./report.htm"


    stage "Publish HTML Reposrt"
    	publishHTML([allowMissing: false, alwaysLinkToLastBuild: false, keepAll: false, reportDir: ‘coverage’, reportFiles: ‘report.html’, reportName: ‘API Test HTML Report’, reportTitles: ‘API Test Report’])
    
}
