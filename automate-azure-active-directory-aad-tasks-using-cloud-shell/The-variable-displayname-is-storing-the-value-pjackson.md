

![automate-azure-active-directory-aad-tasks-using-cloud-shell/](https://www.sqlshack.com/automate-azure-active-directory-aad-tasks-using-cloud-shell/)

## displayname=pjackson

The variable displayname is storing the value “pjackson”. You can verify the value of the variable using the echo command like this:

## Echo $displayname

We will now read user input and store in a variable named password. To do that, run the following command:

## read password

After that, you can write the password, which will be stored in the password variable.

To concatenate values, you just need to write the string together:

## userprincipalname=$displayname@dani671hotmail.onmicrosoft.com

In this example, we are concatenating the variable $dispalyname with the string “@dani671@hotmail.onmicrosoft.com”.

The following example, will use the variables to create a new user:

## az ad user create –display-name $displayname –password $password –user-principal-name $userprincipalname

