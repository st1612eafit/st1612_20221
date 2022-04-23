## Profesor: Edwin Montoya, Universidad EAFIT, Medellín-Colombia
## emontoya@eafit.edu.co

# primeros pasos con ElasticSearch - webinar:

https://www.elastic.co/es/webinars/getting-started-elasticsearch

# instalar:

    AWS EC2: t2.medium / 20 GB DD (si va a usar API REST remoto, recuerde abrir el puerto 9200 y verificar que esta 'oyendo' o listing por 0.0.0.0)

    wget https://artifacts.elastic.co/downloads/elasticsearch/elasticsearch-7.15.1-linux-x86_64.tar.gz

    tar -xzf elasticsearch-7.15.1-linux-x86_64.tar.gz

    cd elasticsearch-7.15.1/

# config: (opcional, primero pruebe iniciar el servidor y si sube bien, no requiere estas opciones)

    set memory:

    https://www.elastic.co/guide/en/elasticsearch/reference/current/vm-max-map-count.html

    $ sudo sysctl -w vm.max_map_count=262144

    $ sudo sysctl -w fs.file-max=65536

# iniciar servidor:

    bin/elasticsearch -d -p pid

# terminar:

    pkill -F pid