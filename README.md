# Overview
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fkonveyor%2Fkonveyor.github.io.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2Fkonveyor%2Fkonveyor.github.io?ref=badge_shield)

This repository contains documentation for projects under [Konveyor.io](http://konveyor.io)
* Leverages [Hugo](https://gohugo.io/)
* Is served at: [https://konveyor.github.io/](https://konveyor.github.io/)
    * Assets are built and served from the branch [gh-pages](https://github.com/konveyor/konveyor.github.io/tree/gh-pages)

# Getting Started, how to run locally
1. Fork or Clone the repository, ensure you check out the configured [git submodules](https://git-scm.com/book/en/v2/Git-Tools-Submodules)
    * Example:

        ``` git clone https://github.com/konveyor/konveyor.github.io.git --recursive```
            
        * We are using the ```--recursive`` command line flag to automatically clone a few themes which Hugo will use.  These are leveraging [git submodules](https://git-scm.com/book/en/v2/Git-Tools-Submodules) 
2. ```cd konveyor.github.io```
3. ```hugo server -D```
    * Run the hugo server locally, building posts that may be in 'draft'
4. Visit http://localhost:1313/ in your web browser

# How changes get published to 'production'

All changes which merge to 'main' will [trigger a GitHub Action](https://github.com/konveyor/konveyor.github.io/actions) to run that builds the hugo assets and publishes to the [gh-pages branch](https://github.com/konveyor/konveyor.github.io/tree/gh-pages) 

The URL,[https://konveyor.github.io/](https://konveyor.github.io/) is configured to serve the web assets from the [gh-pages branch](https://github.com/konveyor/konveyor.github.io/tree/gh-pages)  

## Code of Conduct
Refer to Konveyor's Code of Conduct [here](https://github.com/konveyor/community/blob/main/CODE_OF_CONDUCT.md).

## DCO
Licensing is important to open source projects. It provides some assurances that
the software will continue to be available based under the terms that the
author(s) desired. We require that contributors sign off on commits submitted to
our project's repositories. The [Developer Certificate of Origin
(DCO)](https://probot.github.io/apps/dco/) is a way to certify that you wrote and
have the right to contribute the code you are submitting to the project.

You sign-off by adding the following to your commit messages. Your sign-off must
match the git user and email associated with the commit.

    This is my commit message

    Signed-off-by: Your Name <your.name@example.com>

Git has a `-s` command line option to do this automatically:

    git commit -s -m 'This is my commit message'

If you forgot to do this and have not yet pushed your changes to the remote
repository, you can amend your commit with the sign-off by running 

    git commit --amend -s 


## License
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fkonveyor%2Fkonveyor.github.io.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2Fkonveyor%2Fkonveyor.github.io?ref=badge_large)