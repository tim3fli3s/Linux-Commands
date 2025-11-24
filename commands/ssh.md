ssh user@host
ssh -i key.pem user@host

scp file user@host:/path     # upload
scp user@host:/file .        # download

ssh-keygen -t rsa -b 4096     # create SSH key
