# Using-Multi-GitHub-Account

# https://code.tutsplus.com/tutorials/quick-tip-how-to-work-with-github-and-multiple-accounts--net-22574

# ssh-keygen -t rsa -C "your-email-address"
   ~/.ssh/id_rsa_nettuts
   vim ~/.ssh/id_rsa_COMPANY.pub
   ssh-add ~/.ssh/id_rsa_COMPANY
   
# touch ~/.ssh/config
   vim config   or  code .
# Host github-COMPANY
  HostName github.com
  User git
  IdentityFile ~/.ssh/id_rsa_COMPANY
# Open Your git to remote again
  take the ssh link from repository
  git init
  git commit -am "first commit'
  git remote add origin git@github-COMPANY:Company/testing.git
  git push origin master
