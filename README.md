# CFD - Transwing

There are two methods to compute fluid dynamics of the propeller and transwing.

## MRF-steady

> First, MRF-steady cases for:
>
> - single-propeller.
>
> - semi-fixwing.
>
> - semi-transwing-VTOL.
>
> - full-transwing-VTOL.

## AMI-transient

> Second, AMI-transient cases for single propeller.

## Install OpenFOAM v9

> Add dl.openfoam.org to the list of software repositories for apt to search, and to add the public key (gpg.key) for the repository to enable package signatures to be verified.
>
> - `sudo sh -c "wget -O - https://dl.openfoam.org/gpg.key | apt-key add -"`
>
> - `sudo add-apt-repository http://dl.openfoam.org/ubuntu`

> Update the apt package list to account for the new download repository location
>
> - `sudo apt-get update`

> Install OpenFOAM (9 in the name refers to version 9) which also installs paraviewopenfoam56 as a dependency.
>
> - `sudo apt-get -y install openfoam9`

> User Configuration
>
> - `gedit ~/.bashrc`

> At the bottom of that file, add the following line (see Note 1 below) and save the file
>
> - `source /opt/openfoam9/etc/bashrc`

# References

> https://openfoam.org/download/9-ubuntu/
