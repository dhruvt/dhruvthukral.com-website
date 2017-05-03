#Source files for DhruvThukral.com

Built using MKDocs and deployed using a CI/CD pipeline involving AWS CodeBuild and AWS CodePipeline as a static S3 website.

If you would like to clone this repo to build your own website:

```
	cd ~
	mkdir <your-project-folder>
	cd <your-project-folder>
	pip install virtualenv
    git clone https://github.com/dhruvt/dhruvthukral.com-website.git
    cd dhruvthukral.com-website
    virtualenv website 
```

Once you have the site cloned locally, create your own github repo and change the origin of this repo to your new empty repo

Example: `git config remote.origin.url <your-github-repo-url>`

Example: `git remote add origin <your-github-repo-url>`

Execute a `git push --set-upstream origin master`

Aside: you can now change the name of `dhruvthukral.com-website` local directory to `<new_repo_name>`

To install MKDocs dependencies, execute the following:
```
    source website/bin/activate
    pip install -r requirements.txt
```

To run an auto-updating local copy of your atlas, execute the following:
```
	mkdocs serve
```
You should nw be able to browse to `http://localhost:8000` and see the site. The site will auto refresh in your browser any time a file in your `docs` folder is revised and saved. 
