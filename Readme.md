# RecordoStyle Infra
This repos is responsible for infro setup for recordostyle.com
- S3 bucket
- Cloudfront Distribution with OCA 
- Route 53 (need to update Godaddy NS after deploy)
- Cert (works only after NS updated)
- Api Gateway -> SNS

## Local test POST inquiry endpoint
```
curl -X POST https://api.recordostyle.com/v1/inquiry \
  --data "{'message': 'Hello, from your terminal!'}" \
  -H 'Content-Type: application/json'
```