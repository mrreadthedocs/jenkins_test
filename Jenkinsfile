node('master'){

stage("Test"){
    echo "test"
}

stage("Promote to master"){
    if (env.BRANCH_NAME=='develop'){
        echo "I am a develop brach!"
        sh "git pull"
        sh "git checkout origin master"
        sh "git pull"
        sh "git merge develop"
        sh "git push origin master"
        echo "Code promoted to Master! :) " 
    }
}

}
