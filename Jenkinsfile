node {
        
        checkout scm recursiveSubmodules

    
        stage('Build') {
            echo 'Building....' 
            def files = findFiles(glob: '**/TEST-*.xml') echo """${files[0].name} ${files[0].path} ${files[0].directory} ${files[0].length} ${files[0].lastModified}"""
        }
        stage('Test'){
            echo 'Testing....'
        }
        stage('Deploy dev'){
            echo 'Deploy dev'
        }
        stage('Deploy prod'){
            echo 'Deploy prod'
        }
    
}