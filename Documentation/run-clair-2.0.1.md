# Run Clair v2.0.1 with docker-compose 

    curl -L https://raw.githubusercontent.com/dmitrytokarev/clair/2.0.1/docker-compose.yml -o $HOME/docker-compose.yml
    mkdir $HOME/clair_config
    curl -L https://raw.githubusercontent.com/dmitrytokarev/clair/2.0.1/config.example.yaml -o $HOME/clair_config/config.yaml
    docker-compose -f $HOME/docker-compose.yml up -d