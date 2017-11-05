# Nginx virtualhost creation via docker

It's a very simple script made for an easier management of virtualhost in a containerized nginx.
This script is currently in development version and shouldn't be used in a production environment, there is alot of refactoring needed
to make it work more flexibly with containers.

Keep in mind that its current purpose is to deal with containerized nginx and virtualhost with ease.

A manager has been made for dealing with some recurrent actions:

	- Creation of a new virtualhost via templates.
	- Enabling and disabling virtualhost (add/remove symoblic link from sites-enabled)
	- Deletion of a domain/virtualhost content
	- Files/directories management

The main goal of this script was to allow splitting of a domain into several mini applications via virtualhost.
Once the script works with your environment you can easily create a new virtualhost in a few seconds.

A premature support for composer has been added but need some work to be stable.

This script was initially made for a handmade container named nginx and some lines was written with this in mind, that's
one reason it shouldn't be used in a production environment without checking containers configuration.

I will probably work later on this script to improve it and make it more suitable for multiples production environment.

Keep in mind that it was written last year and docker has changed alot since, so it might not work anymore.
