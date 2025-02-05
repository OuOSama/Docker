# execute
```
docker-compose up -d --build
```

# Create user in MongoDB
```
docker exec -it <replace with container id or container name> mongosh
```
```
use admin
```
```
db.createUser({ user: "root", pwd: "root", roles: [ { role: "root", db: "admin" } ] });
```
# URL
```
mongodb://root:root@localhost:27017/my-db?authSource=admin
```
