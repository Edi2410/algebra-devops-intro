
## run docker compore

    docker compose up -d --build

## build and push latest

    cd tempconverter
    docker build -t tempconverter:latest .
    docker tag tempconverter:latest ghcr.io/edi2410/algebra-devops-into:latest
    docker login ghcr.io
    docker push ghcr.io/edi2410/algebra-devops-into:latest


## build and push dev

    cd tempconverter
    docker build -t tempconverter:dev .
    docker tag tempconverter:dev ghcr.io/edi2410/algebra-devops-into:dev
    docker push ghcr.io/edi2410/algebra-devops-into:dev


## stats 

    docker stats [DOCKER_CONTAINER]
