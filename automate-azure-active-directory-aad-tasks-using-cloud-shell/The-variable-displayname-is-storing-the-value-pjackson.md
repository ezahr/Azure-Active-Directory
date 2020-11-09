

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


## Create multiple Azure Active Directory users from a test file

In the next example, we will create a list of users and we will create AAD users from that list automatically.
We will first create a file named “listuser”. The first line will be ”jlopez”, which is an AAD user that we want to create:

echo “jlopez” > listusers
We will append two more lines to the text file:
echo “dtrump” >> listusers
echo “bobama” >> listusers

You can also specify a password:
read password

The following lines of code will read the file listuser. It will create a user for each line of the file.:

````
cat listusers | while read line
do
az ad user create –display-name $line –password $password –user-principal-name $line@dani671hotmail.onmicrosoft.com
done 
`````
