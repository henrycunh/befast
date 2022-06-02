<div align="right">

### › befast
<sup>little scripts that makes life somewhat easier<sup>

</div>


#### installation
```bash
npm i -g haxx
npx -y degit henrycunh/befast ~/.scripts
 
echo "export PATH=$PATH:$(realpath ~/.scripts)" >> ~/.profile
export PATH=$PATH:$(realpath ~/.scripts)
```

et voilá!

#### scripts

##### `@de`
Runs commands inside a `docker-compose` container. The services must define a `container_name`.


```yaml
# docker-compose.yml
...
services:
  server:
    container_name: my-server
    ...
  db:
    container_name: my-db
    ...
```

```bash
@de server echo "Hello world, but from a container!"
```
