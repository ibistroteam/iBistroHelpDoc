# iBistroHelpDoc
This repository contains all that is needed to fully generate the Knowledge Base of myibistro application.

How to run locally
Make sure to have Ruby installed (Ruby 2.1.x) up.
Install required dependencies with bundle install
Run jekyll serve
Go to http://localhost:4000/help/
How to build in production
This is mostly:

cd ibistro-support
bundle exec jekyll build --destination $target_folder -c _config.yml,_private_config.yml
Private config is used to avoid leaving it in the public repository. Nothing sensitive but I want to make sure nobody deploys it by mistake, in order to avoid affecting our own typekit quotas.
