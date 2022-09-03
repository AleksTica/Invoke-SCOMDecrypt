# Invoke-SCOMDecrypt

## Introduction ##

This tool is designed to retrieve and decrypt RunAs credentials stored within Microsoft System Center Operations Manager (SCOM) databases.

## Pre-requisites ##

To run the tool you will require administrative privileges on the SCOM server. You will also need to ensure that you have read access to the following registry key:

    HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\System Center\2010\Common\MOMBins

You can check manually that you can see the database by gathering the connection details from the following keys:

    HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\System Center\2010\Common\Database\DatabaseServerName
    HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\System Center\2010\Common\Database\DatabaseName

## Usage ##

To run within the PowerShell console:

    powershell.exe -exec bypass
    . .\Invoke-SCOMDecrypt.ps1
    Invoke-SCOMDecrypt
    ...
