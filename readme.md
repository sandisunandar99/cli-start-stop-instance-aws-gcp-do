
### 
this is for example and try to build CLI using golang. 
you can combine with crontab for schedule start stop instance 

## GCP credentials ##
- make sure service accout to client instance only 
```bash
imam@imam-mv:~$ export GOOGLE_APPLICATION_CREDENTIALS=
```

## AWS credentials ##
- make sure iam to allow read only 
```bash
imam@imam-mv:~$ aws configure
AWS Access Key ID [****************XXXX]: 
AWS Secret Access Key [****************XXXX]: 
Default region name [ap-southeast-1]: 
Default output format [None]:
```

## Digitalocean ##
Soon



## How to Use ##
```bash
imam@imam-mv:~$ go build -o ectl
imam@imam-mv:~$ ./ectl aws instance --action=start --region=ap-southeast-1 i-xxx i-xxx
imam@imam-mv:~$ ./ectl gcp instance --action=start --region=sgp i-xxx i-xxx
imam@imam-mv:~$ ./ectl digitalocean instance --action=

```


