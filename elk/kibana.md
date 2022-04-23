## Profesor: Edwin Montoya, Universidad EAFIT, Medellín-Colombia
## emontoya@eafit.edu.co

# primeros pasos con Kibana - webinar:

https://www.elastic.co/es/webinars/getting-started-kibana

# instalar:

    AWS EC2: t2.medium / 20 GB DD (Recuerde abrir el puerto 5601 en la instancia para conectarse remotamente)

    pre-requisito: https://geekflare.com/install-chromium-ubuntu-centos/ (instalar chromium)

    curl -O https://artifacts.elastic.co/downloads/kibana/kibana-7.15.1-linux-x86_64.tar.gz

    tar -xzf kibana-7.15.1-linux-x86_64.tar.gz

    cd kibana-7.15.1-linux-x86_64/

## descomentar en: config/kibana.yml:

    elasticsearch.hosts: ["http://localhost:9200"]
    server.port: 5601
    server.host: "0.0.0.0"

## ejecutar servidor:

    nohup bin/kibana &