# CFD - Transwing

Link repo: https://rtgit.rta.vn/rtr_huylda/cfd_transwing

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

## Install WSL2 on Windows 10
- Search for Command Prompt, right-click the top result, and select the Run as administrator option.
- Type the following command to install the WSL on Windows 10 and press Enter:
    > wsl --install
- Restart your computer to finish the WSL installation on Windows 10.

## Install WSL with Ubuntu distro
- Search for Command Prompt, right-click the top result, and select the Run as administrator option.
- Type the following command to view a list of available WSL distros you can install on Windows 10 and press Enter:
    > wsl --list --online
- Type the following command to install the WSL with a Ubuntu distro on Windows 10 and press Enter:
    > wsl --install -d Ubuntu
- Restart your computer.
## Install OpenFOAM 5.0

> Add dl.openfoam.org to the list of software repositories for apt to search, and to add the public key (gpg.key) for the repository to enable package signatures to be verified.
>
> - `sudo sh -c "wget -O - http://dl.openfoam.org/gpg.key | apt-key add -"`
>
> - `sudo add-apt-repository http://dl.openfoam.org/ubuntu`
>
> Update the apt package list to account for the new download repository location
>
> - `sudo apt-get update`
>
> Install OpenFOAM (5 in the name refers to version 5.0) which also installs paraviewopenfoam56 as a dependency.
>
> - `sudo apt-get -y install openfoam5`

> User Configuration
>
> - `gedit ~/.bashrc`
>
> At the bottom of that file, add the following line (see Note 1 below) and save the file
>
> - `source /opt/openfoam5/etc/bashrc`

# References

> https://openfoam.org/download/5-0-ubuntu/
