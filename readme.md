S3 to S3 transfer
====================================================================================================================================
Create s3 policy in source account for source and destination

Update permission in destination> Edit Object Ownership>ACL enabled> Bucket owner preferred> Apply
Copy single file
  aws copy sync s3://testjovuss3copy/singlefile.txt s3://wtr-images --acl bucket-owner-full-control
Copy multiple file
  aws s3 sync s3://jovus-open-bucket/ s3://wtr-images --acl bucket-owner-full-control

