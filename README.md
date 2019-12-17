# Clarity License Deactivator
This package deactivates users who have not logged in to Clarity PPM for over 90 days.

## Business Reason
It helps you saving costs, since deactivated users do not consume licenses on Clarity.

## How does it work?
It implements a process called Deactivate Users which you can both manually run through the Organizer feature or create a recurring job to automatically trigger the process. Do not forget to activate this process after installing this package.

## How to install
- Make sure you have the XOG client installed on your machine
- Download the latest release of Clarity License Deactivator package [HERE](https://github.com/thiagobottoni/Clarity-License-Deactivator/releases)
- Extract the zip file to your C:\temp directory
- Open the file cld_install.bat
- Inform the correct values to the following variables: 
  - XOG_HOME = XOG client installation directory, i.e. c:\apps\xog\bin
  - SERVERNAME = Clarity hostname or IP, i.e. cappm1561
  - PORTNUMBER = Clarity port, i.e. 80, 443
  - SSLENABLED = Inform if Clarity is running over HTTPS or not, i.e true or false
  - USERNAME = User with XOG rights, i.e. admin, xog
  - PASSWORD = User password
- Save and close the file
- Run the file cld_install.bat
- Check the output file for errors at C:\temp\cld_install\output

## Languages
This release is available in two languages: English and Brazilian Portuguese.

## Important
- It works for On Premise customers only, even if you use LDAP, SSO or Clarity user directory! It does not work for SaaS customers, since Broadcom On Demand Portal has its own user directory system.
- This package was built for Oracle database. If you use SQL Server, you have to adapt the SQL queries inside the GEL script.
