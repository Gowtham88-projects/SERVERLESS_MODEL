Now many people are getting error in different stages I will explain how i did troubleshooting:
1. Everyone while you are creating dynamodb table and partition key please keep name as shown in video otherwise you will have to make changes in scripts applicable only if you are using code from this video.
2. I have created role for lambda function and given them full access to dynamodb and api gateway
3. In get function script do change the region 
4. While testing event in lambda for insert function please check format of your json otherwise you will get errors
5. After creating api gateway do add endpoint in js file and do click on deploy.
6. After uploading my files in s3 bucket and attaching policy i was able to open my website but i was not able perform any action as i was getting popup about error. After checking in inspect > console i got cors related error. You have to attach cors policy for you s3 bucket
policy : 
7.  we are accessing the website from S3 so it is not secure so fr to get more secure to our website here i deployed an Website infront of S3
8.  so now our student data website is  Secure.
