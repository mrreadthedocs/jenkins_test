node('master'){

stage("Test"){
    echo "test"
}

stage("Checkout SCM"){
    checkout scm
}

stage("Promote to master"){
    if (env.BRANCH_NAME=='develop'){
        echo "I am a develop brach!"
        sh "pwd"
        sh "git checkout master"
        sh "git pull"
        sh "git merge develop"
        sh "git push"
        echo "Code promoted to Master! :) " 
    }
}

}
