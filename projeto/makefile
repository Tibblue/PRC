.PHONY: backend frontend
.PHONY: graphdb json_server
.PHONY: runAllBackground
.PHONY: kill

# 1205  docker commit hungry_pascal tibblue/graphdb_prc:v3.0
# 1207  docker push tibblue/graphdb_prc:v3.0
# 1213  docker run -p 7200:7200 tibblue/graphdb_prc:v3.0
# 1245  docker image rm -f tibblue/graphdb_prc:v3.0

### Runners
# exec backend (Node)
backend :
	cd backend && \
	nodemon start

# exec frontend (Vue)
frontend :
	cd frontend && \
	npm run serve

# exec GraphDB (using docker)
graphdb :
	docker run -p 7200:7200 tibblue/graphdb_prc:v3.0

# exec json-server (User Database)
json_server :
	cd usersdb && \
	npm run json:server

# exec backend & frontend (in background)
runAllBackground :
	cd backend && \
	nodemon start &
	cd frontend && \
	npm run serve &

### Killers
kill :
	killall -SIGKILL node
	killall -SIGKILL npm
	killall -SIGKILL sh
