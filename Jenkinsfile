node {
  stage('do something with git') {  
    sshagent (credentials: ['github-key']) {
      // get the last commit id from a repository you own
      sh 'git ls-remote -h --refs https://github.com/suraj-sbrt/nodejs.git master |awk "{print $1}"'
    }
  }
}
