Projeto Destinado ao aprendizado do consul da Hashcorp


###Comandos## 
docker container run -it consul:1.9.4 sh

abrir um novo terminal
$docker ps
$docker exec -it nomedocontainer sh

$consul members

$netstat -napt (visualizar as portas)

$curl localhost:8500
$curl localhost:8500/v1/catalog/nodes
$apk -U add bind-tools
$dig @127.0.0.1 -p 8600 nomedoContainer.node.consul

###
1 - Subir um containet com o consul
2 - instalar o dig - $apk -U add bind-tools
$consul agent -dev -config-dir ./consul.d
