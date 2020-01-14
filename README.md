# grok-exporter v1.0.0.RC2 with multi log files 


## how to running

*  start docker services

```code
docker-compose up -d 
```


* append logs

```code
touch  example/rong.log
touch  example/examples.log
echo "30.07.2016 14:37:03 alice 1.5" >> example/rong.log
echo "30.07.2016 14:38:03 alice 1.5" >> example/rong.log
echo "30.07.2016 14:39:03 rong 1.5" >> example/examples.log
```

* view metrics

```code
open http://localhost:9144/metrics
```