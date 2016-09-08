# .Net_FtpClient
Small and basic ftp client to c#

# How to Use
Add using to header
```c#
  using com.ocampogeric
```

create an object of FtpClient class

```c#
FtpClient ftpClient = new FtpClient();
  //Set required attributes
  ftpClient.Host = "ftp://<your host here>";
  ftpClient.User = "username";
  ftpClient.Pass = "***********";
  //Example to use methods
  try{
  ftpClient.uploadByteArray("/dir/Test.txt", yourByteArray); //Byte[] is required
  }catch(Exception ex){
    do something with ex
  }
```

## Attributes
- Host
- User
- Pass
- Passive `//this set passive mode`


###### The Licenses are in LICENSE file
