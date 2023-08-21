## Task
This is step-by-step process of how to create a user, add user to a group, and grant certain permissions. This is in fulfillment to a task given by my instructor at AltSchool Africa for the Cloud Engineering Program. 

Before I begin, I've already installed the following:
- Virtualbox
- Ubuntu 0S 

### Create a user
Run the following command on your Ubuntu terminal:

```sudo adduser YOUR-USERNAME```

Output:
<img src="./screenshots/add-user.png"  width="100%" height="100%">

### set an expiry date of two weeks for the user
The way to set an expiry date for a user is by running 

``` sudo chage -E yyyy-mm-dd YOUR-USERNANE```

Output:
<img src="./screenshots/expirydate.png"  width="100%" height="100%">

### Verify that the expiry date has been set
To verify the expity date, run: 

```sudo chage -l YOUR-USERNAME```

You should have a similar output as this:
<img src="./screenshots/verify.png"  width="100%" height="100%">

### Prompt the user to change password on login

<img src="./screenshots/change-password.png"  width="100%" height="100%">

<img src="./screenshots/switch-user.png"  width="100%" height="100%">

### Attach the user to a group called "altschool"

<img src="./screenshots/add-group.png"  width="100%" height="100%">

<img src="./screenshots/group.png"  width="100%" height="100%">

### Allow altschool group to be able to run only `cat` command on /etc/

<img src="./screenshots/cat.png"  width="100%" height="100%">


### Create another user. make sure that this user doesn't have a home directory.

<img src="./screenshots/no-home.png"  width="100%" height="100%">

### Verify
<img src="./screenshots/switch-to-user2.png"  width="100%" height="100%">