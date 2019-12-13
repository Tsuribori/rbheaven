## RBHeaven

Site for discussing anything, anonymously.

### Development

```
docker-compose -f docker-compose.dev.yml up --build
```

### Production

Switch the environment variables in `docker-compose.yml` to your needs.
Replace instances of `server_name example.com;` in `nginx/prod/local.conf` to your own domain.

```
docker-compose up --build
```
