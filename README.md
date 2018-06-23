# Testing semantic version using https://github.com/GitTools/GitVersion.

## Quite easy to implement in your projects.

### commands history, playing around: 

   75  git clone git@github.com:markchalloner/git-semver.git
   76  cd git-semver/
   77  git checkout
   78  git tag | grep '^[0-9]\+\.[0-9]\+\.[0-9]\+$' |     sort -t. -k 1,1n -k 2,2n -k 3,3n | tail -n 1
   79  sudo ./install.sh
   80  cd ..
   81  ls -la
   82  cd svAngular6/
   83  ls -la
   84  git semver get
   85  sudo git semver get
   86  git init
   87  sudo git semver get
   88  git semver patch|next
   89  sudo git semver get
   90  git semver minor
   91  sudo git semver minor
   92  git remote add origin https://github.com/thiswallz/angular6SemanticVersion.git
   93  git push -u origin master
   94  git status
   95  git add .
   96  git commit -m "First commit"
   97  git push -u origin master
   98  sudo git semver get
   99  git semver patch|next
  100  sudo git semver patch|next
  101  sudo git semver get
  102  sudo git semver patch|next
  103  sudo git semver get
  104  git status
  105  vim src/app/app.module.ts 
  106  sudo git semver patch
  107  git status
  108  git add .
  109  git commit -m "Modify module"
  111  git status
  112  git push -u origin master
  113  git push origin --tags
  114  vim src/app/app.module.ts 
  115  git status
  116  git add .
  117  git commit -m "Add function to module"
  118* git
  119  git push -u origin master
  120  git push origin --tags
  121  vim src/app/app.module.ts 
  122  sudo git semver major
  123  git status
  124  git add .
  125  git commit -m "Change name add function"
  126  git status
  127  git push -u origin master
  128  git push origin --tags
  129  sudo git semver minor
  130  git push origin --tags
  131  vim src/app/app.module.ts 
 
### summarizing this last part is like everything you need , just select patch/minor/major/etc

  132  git add .
  133  git commit -m "Add other function"
  134  sudo git semver minor
  135  git push -u origin master
  136  git push origin --tags
  137  history

