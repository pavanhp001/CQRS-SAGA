# CQRS-SAGA
CQRS-SAGA in microservices

Run Axon in docker 
https://developer.axoniq.io/w/running-axon-server-in-docker-continuing-from-local-developer-install-to-containerized


https://github.com/simplyi
https://github.com/simplyi/ProductsService
https://github.com/simplyi/OrdersService
https://github.com/simplyi/core
https://github.com/simplyi/PaymentsService
https://github.com/simplyi/ApiGateway
https://github.com/simplyi/DiscoveryService

Lombok error in STS IDE
https://stackoverflow.com/questions/11803948/lombok-is-not-generating-getter-and-setter/45217235#45217235

axonserver.properties
===================
server.port=8024
axoniq.axonserver.name=My axonserver
axoniq.axonserver.hostname=localhost
axoniq.axonserver.devmode.enabled=true

to execute axon server using docker 
=================================

docker run -d --rm --name axonserver -p 8024:8024 -p 8124:8124 -v "F:/MService-WS/CQRS-SAGA/AXONFW/axonserver/data":/data -v "F:/MService-WS/CQRS-SAGA/AXONFW/axonserver/eventdata":/eventdata -v "F:/MService-WS/CQRS-SAGA/AXONFW/axonserver/config":/config axoniq/axonserver
