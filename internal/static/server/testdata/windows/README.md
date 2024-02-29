The files here are for usage with windows TLS. They need to be installed to the Users certificate store in the `My` location if using the included agent configuration. 

Running ` .\curl.exe -v -GET --key .\client_key_unencrypted.key --cert .\client_cert.crt --insecure https://localhost:12345/metrics` will let you see the correct metrics. NOTE: You will need to likely download [curl](https://curl.se/windows/dl-7.82.0_2/curl-7.82.0_2-win64-mingw.zip) compiled explicitly with windows crypto support. 