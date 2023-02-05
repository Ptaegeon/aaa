# Zip file unzip

# tar file untar

# wget download
``` python

import wget

session = '001'
url = 'https://dcapswoz.ict.usc.edu/wwwdaicwoz/{}_P.zip'.format(session)
directory_path = 'C:\...'
wget.download(url, directory_path)
```
