[github for beginners](https://www.youtube.com/watch?v=RGOj5yH7evk)
### git push
---
what if you want to create a repo locally

But what about if   you start a repo locally, so let me exit out 
of these. And I will create a new folder here   called demo repo to drag it outside. So now it's 
in a completely separate folder from the other   Git repository that we have. But this one's 
not a git repository yet, and nothing's in   there. 

So I'm going to move into that folder in the terminal. Demo two. So now I'm in demo two,   you can see it's not a git repository. Even if I look for that hidden Git folder, it's not there.   

So let me first add a file in here. And I'm again, going to add a readme file that MD and  

**00:27:16**

I'm going to add a header demo to and some text. 

Now, if I want to turn this into a git repository,   

I can use the command line and say Git init.
```
git init 
```

And it says initialize Git repository in yada yada,   this folder, and now you can see I have the 
git keyword there. 

And if I do get status,   I can see there's this untracked README file, I 
will go ahead and add that file, either with the   period or the name of the file.
```
git status

```

git status again, 
okay, so the file is ready to be committed. 

And   now I will do git commit dash m, created README. 
```
git commit -m "created README"

```

And now I'll put a description here, and Enter.   

Now what if I want to push this live? Let's try 
git push origin master.
```
git push origin master

```
And now you can see it's   giving me this error ``` **fatal origin does not appear 
to be a git repository ** ```. Because we didn't clone   this down from a git repository. 

We didn't already create this repo on GitHub, we created it locally.   

So Git is saying I have no idea where to push this to because it's not connected to anything. So we   have to create that connection. And first, the easiest way to do this is by creating an empty   Git repository up on GitHub. So I'm going to come 
here, create new repository, I'm going to call  

**00:28:50**

This **demo-repo2** to don't need a description, going 
to leave all this here. Now I have another empty   repository. 

So to start pushing here, I'm going 
to copy this and say Git remote, now remote mean   somewhere else, but not on this computer. We're 
going to use this to add a reference to the remote   repository on GitHub. And then I'm going to say 
add origin and paste that link that I copied. 

And   I can check that by saying ``` Git remote dash V ```,


and it shows any remote repositories that I've   connected to this repo. Now that these are set up. 

I can now use ```git push origin, Master``` just as I   did before. 

Now, there's a shortcut here, because 
if I don't want to type out this whole thing,   every time in the future, I can just use ``` git push```, 
but I have to set ```something called an upstream```,   meaning this is where I want to push it to 
by default. So I'm going to do dash u for set   upstream and then enter In the future, I can just 
use git push without typing out origin Master,   it says to GitHub looks like everything was 
pushed just fine, I will refresh this page,   


and I can see the readme that I just added. So 
that's how you initialize a repository locally and  

**00:30:18**

Push it to a remote location like GitHub. 

So let's 
review the workflows that we've gone over so far,   and compare the flow of adding code in the 
GitHub interface versus writing it locally.   So when we first started working in the GitHub 
interface, we wrote some code in the readme,   and then we committed our changes we saved them 
to get now notice, there wasn't an added step   here. And we never did a git add to stage changes. 
Well, that's because GitHub handles that for us.  

So really, by committing in GitHub, we are adding 
and committing at the same time. 

And then that was   it really, because it was our repository, we 
had full access to change whatever we wanted,   we could just update the code just by committing 
it in the GitHub interface. Of course, we didn't   have to push the code because it was already live 
on GitHub.

There's no other remote repository,   because it's already in the remote repository. 


Now, if we didn't own the repository, or we didn't   have access rights, or we needed other people 
to review our code, before we merged it in with   all the rest of the code, then we would also have 
to take the extra step of making a pull request,  




# Forking

One more thing that I want to quickly mention is   forking, you may have seen this already in 
the Git interface, you can hit fork here,   and then it's going to ``` make a complete copy of the 
repository``` .

Now, why would you want to fork? Well,   you probably don't want to fork your own repo 
because you already have full access to all of the  

01:02:10

Code here, but you don't for other people's repos. 


So let me find just a random repo on GitHub. Okay,   so here's vue.js. So let me click on this. And 
I actually don't have access to change anything   in this repo. 

- So if I want to make a PR against 
this repo, and request for my changes to be added,  
- or if I just want to be able to branch off of the 
code in this repo and do whatever I want with it,   then I want to fork it.

So I'm going to hit the 
fork button here and fork it to my user account.   

These are just groups that I'm a part of on 
GitHub. 

Sometimes it takes a minute to fork   over all the code, especially with Vue JS because 
it's a large repository.

Alright. And now you can   see the repo is no longer under the vue.js 
organization.

Now it's under my personal GitHub.  

And now that I've forked this, I have complete 
control to make any updates or changes that I   want to this code. So if I want to come in to read 
me, and hit the pencil, update this, I can say, Hi   there. 

And now I can come to the bottom and commit 
changes again. So I can say, updated README or   whatever I want, I'm just going to leave it with 
the default text, again, commit to the dev branch.  

01:03:41

So before we worked off the master branch as being 
the default branch, but sometimes when you're   working in a larger project with other people, 
you're going to want to create multiple branches,   like master staging, and dev for different kinds 
of environments. So in this case,

Dev is set to   the default branch for this repository, instead 
of master. So I'm just going to commit my changes   directly to Dev.

And you can see my changes here. 
Of course, they aren't part of the main view j s   view repository, but they're part of the one that 
I forked because I forked a complete copy of that   repository, including the branches associated with 
it. 
And you can see dev is marked as the default.   

So now what if I wanted to get my changes back 
into this Vue JS repository? Of course I don't,   but what if I did, I would go and create a pull 
request. 

So new pull request, and then as my base   the place that I want to merge my changes into I 
would put the repository that I forked from this   Vue JS repository, and the branch and I want to 
compare that with My repository that I forked   and the branch on my repository that I updated, 
of course, I'm not going to click Create pull  

01:05:07

Request, because this is just a demo, I can also 
see the diff down here of the changes that have   made and what commits I've made to this branch on 
my fork.

# Now, if I want to merge within my fork,   I can do that easily. 

Let's say, of course, there 
isn't anything to compare because I'm comparing   the same branch here. But I could merge into any 
other branch. Let me find master here. 

```So I could   merge straight into master. ```

And you can see I 
can create pull requests. 

Now, I created a pull   request. And I'm going to create pull request. 
And you can see they had a bunch of default text   added to the pull request information. 

But I'm 
just going to go ahead and merge. Go back to the   code. If I scroll down, of course, ``` I'm on Dev```, 
it says hi there. 

```And now if I go to master```,   it also has my changes on master because I merged 
them. 
Generally speaking, after we merge a branch   into one of our default branches like Master, 
then we would clean up the branch that has just   been merged. 

In other words, we would delete 
it from GitHub and from our local machine,   because we're not using that branch anymore. But 
it's a little bit different when we use branches  

01:06:32

Like Dev, staging and master, because generally, 
you're merging your feature branches into either   dev or master. And you have Dev and master and 
sometimes staging reserved for just merging into   so you don't make any changes on Dev and master 
themselves. You'll just be merging other branches   into dev or Master, depending on how your codebase 
is set up. In a large project like Vue js,   we would merge all of our feature branches or bug 
fixes or whatever into the dev branch and then   delete the branch that we just merged in. And then 
when all the changes on the dev branch are ready,   those get merged into master. 

But dev never gets 
deleted, just like master never gets deleted,   those kind of stay around forever. All the other 
branches are just temporary. So me having my own   fork allows me full rein, full access, full 
control of CRUD operations, create, read,   update, delete whatever I want to do with all 
of this code, all of these files. And if I want   to make some major updates, what I'm going to 
do is fork the repository, which I already did,   

``` 
pull my fork down to my local machine, make all 
the updates that I want to test them out whatever  
```

01:07:47

I want to do, I'll push them back up to my fork, 
and then I will create a PR against the original   repository.
