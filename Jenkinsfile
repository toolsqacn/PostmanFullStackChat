node {

    checkout scm

    stage "CRMS API Test"
    
        sh "newman run epmployee.postman_collection.json --reporters cli,html --reporter-html-export ./report.htm"
    
    
    
}
