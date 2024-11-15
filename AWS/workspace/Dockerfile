family: my-web-app
containerDefinitions:
  - name: my-web-container
    image: my-docker-image:latest
    memory: 512
    cpu: 256
    essential: true
    portMappings:
      - containerPort: 80
        hostPort: 80
    logging:
      logConfiguration:
        logDriver: awslogs
        options:
          awslogs-group: /ecs/my-web-app
          awslogs-region: us-east-1
          awslogs-stream-prefix: ecs




# docker build -t my-docker-image .
# docker tag my-docker-image:latest 123456789012.dkr.ecr.us-east-1.amazonaws.com/my-repository:latest
# docker push 123456789012.dkr.ecr.us-east-1.amazonaws.com/my-repository:latest
