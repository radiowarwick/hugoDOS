+++
title = "User Management"
chapter = true
weight = 102
+++

# User Management

User Management can be done from the `raw` server. Using this you can create users, sync accounts from the union database, reset passwords, etc.
All of the scripts can be found in the directory `/usr/local/mgmt` and the scripts need to be run as `root` or using `sudo`.

## Scripts

| Script Name | Function |
| --- | --- |
| `socresetpasswd <username>` | Emails given user with a new random password |
| `socpasswd <username>` | Changes the users password to that given |
| `socadduser` | Create a new user interactively. Requires: student number, surname, forename, email |
| `socaddgroup` | Creates a new user group given in the prompt |
| `socaddtogroup` | Adds user(s) to the groups given |
| `socaccess` | User account enabling/disabling. Run script for usage instructions |

## Unix Groups

User groups are used for access to the department folders. These can be found in `/dept` on `raw`.

A list of users of a group can be obtained by running `getent group "<group name>"`. A users group membership can be obtained by running `groups <username>`.

| Group Name | Who? | Details |
| --- | --- | --- |
| Domain Admins | Tech Exec | Gives sudo rights across the network & admin on windows machines
| Domain Users | Every User | |
| it | Tech Exec | Gives access to `/dept/it` and access to `dps0` server |
| rawwwww | Tech Exec | Gives access to the database online https://space.radio.warwick.ac.uk/phppgadmin
| news | Head of News, Station Manager | Gives access to `/dept/news` |
| arts | Head of Arts, Station Manager | Gives access to `/dept/arts` |
| sport | Head of Sport, Station Manager | Gives access to `/dept/sport` |
| speech | Head of Speech, Station Manager | Gives access to `/dept/speech` |
| production | Head of Production, Publicitys, Station Manager | Gives access to `/dept/production` & `/dept/library` |
| publicity | Head of Production, Publicity, Station Manager | Gives access to `/dept/publicity` |
| sponsorship | Head of Sponsorship, Station Manager | Gives access to `/dept/sponsorship` |
| training | Head of Training, Station Manager | Gives access to `/dept/training` |
| raw-admin | Programme Controller, Treasurer, Station Manager, Secretary | Gives access to `/dept/admin` |