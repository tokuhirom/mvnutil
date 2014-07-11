# NAME

mvnutil - tiny utility command for Apache maven.

# SYNOPSIS

    % mvnutil release
    % mvnutil docs
    % mvnutil help

# DESCRIPTION

Apache maven is really awesome framework for managging dependencies. But it's really painful when I release the libraries on maven central repository. I want to release it on the github pages.

This command help to manage maven repo on gh-pages!

# PREPARATION

You need to clone your maven repository in ~/.mvn-release/ directory before working.

    git clone git@github.com:tokuhirom/maven.git ~/.mvn-release/
    git checkout gh-pages

If you don't have a repository to work, run the following commands

    mkdir -p ~/.mvn-release/
    cd ~/.mvn-release/
    git init
    touch README.md
    git remote add origin git@github.com:your/repository.git
    git checkout -b gh-pages
    git push -u origin gh-pages
