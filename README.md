WordPressDemo
=============

WordPress app for various Demos

Current version = 3.7.1 ( as of Dec 12 2014 )

Requirements
------------
Tested in AWS Elastic Beanstalk in 64bit Amazon Linux 2013.09 with PHP 5.4 and 5.5. Should work fine in newer as well.

Changes
------------
The only thing different from the basic WordPress release mentioned is an update to the wp-config.php to make the variables for database connectivity to be based off of $_SERVER variables that get passed in. This can be easily done with Elastic Beanstalk Environment parameters.

<table>
  <tr>
    <th>Variable Name</th>
    <th>Varialbe Value/Default</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>DBName</td>
    <td>ebdb</td>
    <td>Name of the database to use. "ebdb" Is the Elastic Beanstalk default using the eb cli tool.</td>
  </tr>
  <tr>
    <td>DBuser</td>
    <td>ebroot</td>
    <td>User in the database to use. "ebroot" is the Elastic Beanstalk default using the eb clie tool.</td>
  </tr>
  <tr>
    <td>DBPass</td>
    <td>no default</td>
    <td>You set this when you create the DB/Elastic Beanstalk environment.</td>
  </tr>
  <tr>
    <td>DBHost</td>
    <td>no default</td>
    <td>This is the DNS name of the DB instance to connect to.</td>
  </tr>
</table>


