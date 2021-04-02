curl -XPOST "http://localhost:9000/2015-03-31/functions/function/invocations" -d '{}'
docker run -p 9000:8080 aaaa:latest

aws ecr get-login-password --region ap-southeast-2 | docker login --username AWS --password-stdin 950765595897.dkr.ecr.ap-southeast-2.amazonaws.com

aws ecr create-repository --repository-name aaaa --image-scanning-configuration scanOnPush=true --image-tag-mutability MUTABLE

docker tag aaaa:latest 950765595897.dkr.ecr.ap-southeast-2.amazonaws.com/aaaa:latest


docker push 950765595897.dkr.ecr.ap-southeast-2.amazonaws.com/aaaa:latest