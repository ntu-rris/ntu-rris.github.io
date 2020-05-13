---
title: bitbucket/gitlab users
author: milton choo
---
upload to ntu-rris from bitbucket/gitlab

inorder to update from another git based repository to RRIS's github repository
please ensure the following:

* your github account has 2FA with NTU's enterprise authentication server
* your new repository is created on ntu-rris central repository
* optional but highly recommended that you get Single-Sign-On (SSO) to work with github
* on your local git repository, add RRIS's github URL as a "SSH" connection to ntu-rris's with name as "rris", assuming the origin name was taken for bitbucket or gitlab.
{% highlight ruby %}
    $ git remote add rris ssh://git@github.com/ntu-rris/yournewrepositoryname.git
{% endhighlight %}
* push the master branch using this command
{% highlight ruby %}
    $ git push rris master
{% endhighlight %}

it is also recommended that you update the central repository at least weekly for all your active projects
