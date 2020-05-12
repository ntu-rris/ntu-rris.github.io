---
---

upload to ntu-rris from bitbucket/gitlab

inorder to update from another git based account to RRIS's github repository
please ensure the following

* Ensure your github account has 2FA with NTU's enterprise authentication server
* Ensure that your new repository is created on ntu-rris central repository
* Add RRIS's github URL as a "SSH" connection to ntu-rris's with name as "rris"
{% highlight ruby %}
    $ git remote add rris ssh://git@github.com/ntu-rris/yournewrepositoryname.git
{% endhighlight %}
* push the master branch using this command
{% highlight ruby %}
    $ git push rris master
{% endhighlight %}
