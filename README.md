# This project using Python and deployment with AWS EKS


## Application Port
`Port application running on 2000`

<<<<<<< HEAD
## Environment Variable for Apps

- AWS_ACCESS_KEY_ID=your access key id
- AWS_SECRET_ACCESS_KEY=your secret access key
- AWS_SESSION_TOKEN=your session token
- AWS_REGION=your default region
- ATHENA_DB=your db athena
- S3_STAGING_DIR=your s3 bucket
- FLASK_SECRET_KEY=lks
- API_GATEWAY_URL=your url api gateway
- SNS_TOPIC_ARN=your sns topic
- ATHENA_SCHEMA_NAME=your db athena


## Environment for Github Action
- AWS_ACCESS_KEY_ID=your access key id
- AWS_SECRET_ACCESS_KEY=your secret access key
- AWS_SESSION_TOKEN=your session token
- AWS_REGION=your default region
- ECR_REGISTRY= your ecr registry id
- ECR_REPOSITORY = your ecr name
- CLUSTER_NAME = your name cluster EKS

## Install Dependencies
`pip install -r requirements.txt`

## 📊 Query Athena

### ✅ Query: CREATE EXTERNAL TABLE

```sql
CREATE EXTERNAL TABLE IF NOT EXISTS rekognition_results_db.rekognition_results_table (
  image_key string,
  labels array<struct<Name:string, Confidence:double>>
)
ROW FORMAT SERDE 'org.openx.data.jsonserde.JsonSerDe'
WITH SERDEPROPERTIES (
  'serialization.format' = '1'
)
LOCATION 's3://your-destination-bucket/results'
TBLPROPERTIES ('has_encrypted_data'='false');
=======
## Environment Variable

`AWS_ACCESS_KEY_ID=your access key id`<br/>
`AWS_SECRET_ACCESS_KEY=your secret access key`<br/>
`AWS_SESSION_TOKEN=your session token`<br/>
`AWS_REGION=your default region`<br/>
`ATHENA_DB=your db athena`<br/>
`S3_STAGING_DIR=your s3 bucket`<br/>
`FLASK_SECRET_KEY=lks`<br/>
`API_GATEWAY_URL=your url api gateway`<br/>
`SNS_TOPIC_ARN=your sns topic`<br/>
`ATHENA_SCHEMA_NAME=your db athena`<br/>

## Install Dependencies
`pip install -r requirements.txt`
>>>>>>> a5129244e1fb687b958df930a3d59d337f356f93
