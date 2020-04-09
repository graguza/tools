# Tools
Things that I do not want to loose.

## Certificates
It requires following:
* makecert.exe
* pvk2pfx.exe

Both makecert and pvk2pfx are part of [Windows 10 SDK](https://developer.microsoft.com/pl-pl/windows/downloads/windows-10-sdk/).

How to generate self-signed:

* CA Certificate - [see CreateCARoot.bat](/certificates/CreateCARoot.bat)

   ```shell
   CreateCARoot.bat [ca]
   # ca - your ca name
   ```

* SSL Certificate - [see CreateSSLCertificate.bat](/certificates/CreateSSLCertificate.bat)

   ```shell
   CreateSSLCertificate.bat [filename] [password] [cn]
   # filename - name under which files will be saved
   # password - certificate password
   # cn - certificate comma separated common names e.g. CN=computername.domain.com, CN=localhost, CN=computername
   ```
