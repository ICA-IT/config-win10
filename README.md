# config-win10
Configure various Windows 10 settings like lockscreen, hibernationboot, telemetry sending and update behavior.

Danger! Danger! Will Robinson!  :  Do not use on a Windows Domain client or if you ever intend to join the
computer to a domain. It will prevent the domain control of certain settings.

Note regarding the Rev 4.1.2-9 update: if the previous version is already installed on your server, you will
need to include the "-p package" option on your opsi-package-manager command. This revision changes the defaults
for the package properties. The opsi-package-manager will not update defaults on an existing package unless
explicitly instructed to. If you don't see the defaults for the parameters change when running configed, the
problem is likely due to not using the "-p package" option when running opsi-package-manager the first time
after the update. See man opsi-package-manager for details.
