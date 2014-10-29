ssh-environment-themes
======================

Changing Terminal color per environment

Move the ssh file in path ~/bin/ssh and add in your ~/.bash_profile the code line below:

export PATH=$HOME/bin:/opt/local/bin:$PATH

Restart your Terminal or execute the command:

~user$ source ~/.bash_profile

Done!

--------------------------------------------------------------------------------------------------

When you type the commands below, your Terminal will change the Theme, I give some examples:

~user$ ssh qa 1
The Terminal change to Homebrew and acess ssh hostname configured in file ssh.

~user$ ssh prod 3
The Terminal change to Pro and access ssh hostname configured in file ssh.

You can modify the name of environments like staging, qa, production and etc.

--------------------------------------------------------------------------------------------------

In file ssh... You can see:

Between lines 23-27 change to default theme (Basic) when user quit from environment who was logged or when he press Crtl + C.
The lines 3-4 defines properties about Q.A environment and you theme.
The lines 6-7 defines properties about Production environment and you theme.
The lines 31-33 use properties variable qa
Between lines 37-46 use properties variable prod and there are a simple validation to confirm access in production environment.

That's all!

Thanks.
