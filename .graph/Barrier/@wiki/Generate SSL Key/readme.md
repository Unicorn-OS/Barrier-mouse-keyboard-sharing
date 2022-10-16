# Linux
https://github.com/debauchee/barrier/issues/965

# Windows
https://github.com/debauchee/barrier/wiki/Command-Line#ssl_config

# Pull Request:, try:
## Q: Error in Windows:
`ssl certificate doesn't exist: C:\Users\<username>\AppData\Local\Barrier\SSL\Barrier.pem`**
A: Use WSL2 to install `openssl` and generate SSL key

`openssl req -x509 -nodes -days 9999 -subj /CN=Barrier -newkey rsa:4096 -keyout Barrier.pem -out Barrier.pem`

https://github.com/debauchee/barrier/pull/1753

