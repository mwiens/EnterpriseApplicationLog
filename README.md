# EnterpriseApplicationLog
Enterprise Application Log with RabbitMQ, LogStash, ElasticSearch and Kibana

## How to use
```
git clone https://github.com/docker-gallery/EnterpriseApplicationLog.git
cd ./EnterpriseApplicationLog
docker-compose up
```

## Result

### RabbitMQ
- New and default *virtual host* ```EnterpriseLog``` will be created automatically
- Use **[http://localhost:15672/](http://localhost:15672/)** for management with **User**: ```logUser``` and **Password**: ```logPwd```

### ElasticSearch
- Will be used to storage Log content

### LogStash
- Are configurated do **create** ```ApplicationLog``` *queue* on ```EnterpriseLog``` *virtual host* and listen this queue
- Every message in ```EnterpriseLog/ApplicationLog``` will be send to ```ElasticSearch```

### Kibana
- Was configurated do read ```ElasticSearch```
- Use **[http://localhost:5601/](http://localhost:5601/)** for management without credentials

# Enjoy!
more content like that you will see on:
- [Website / Blog](http://luizcarlosfaria.net/)
- [YouTube](https://www.youtube.com/luizcarlosfaria/)
- [Facebook Page](https://www.facebook.com/ArquitetoDeSolucoes/)
- [Facebook Group](https://www.facebook.com/groups/arquiteturadotnet/)

All content still produced in PT-BR language. To request an english version, please send me a message on [twitter](https://twitter.com/luizcarlosfaria) or [email](mailto:luizcarlosfaria@gmail.com).
