# AwsCLI
AwsCli for S3 Bucket

🐧 Install AWS CLI on Linux (Ubuntu / Debian / aws Linux)


1️⃣ Install Python (if not already installed)
sudo yum update -y
sudo yum install awscli -y
sudo apt update
sudo apt install python3 python3-pip -y
python3 --version

2️⃣ Install AWS CLI (v2)
curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
unzip awscliv2.zip
sudo ./aws/install

✅ Verify:
aws --version


🔧 Configure AWS CLI
aws configure

You will be prompted for:

AWS Access Key ID [None]: <YOUR_ACCESS_KEY>
AWS Secret Access Key [None]: <YOUR_SECRET_KEY>
Default region name [None]: us-east-1
Default output format [None]: json


AWS Access Key ID     : YOUR_ACCESS_KEY
AWS Secret Access Key : YOUR_SECRET_KEY
Region                : ap-south-1  # Example: Mumbai
Output Format         : json


✅ Test AWS CLI:

📦 Create an S3 Bucket:
  aws s3api create-bucket \
  --bucket mybucketatulkamble2 \
  --region us-east-1

  ✅ You should get JSON response confirming the bucket creation.

  🔍 List Buckets:

  aws s3 ls
