## Profesor: Edwin Montoya, Universidad EAFIT, Medellín-Colombia
## emontoya@eafit.edu.co

# primeros pasos con ElasticSearch - webinar:

https://www.elastic.co/es/webinars/getting-started-logstash

# instalar:

    AWS EC2: t2.medium / 20 GB DD

    wget https://artifacts.elastic.co/downloads/logstash/logstash-7.15.1-linux-x86_64.tar.gz

    tar -xzf logstash-7.15.1-linux-x86_64.tar.gz

    cd logstash-7.15.1

    bin/logstash -f etl-file.conf