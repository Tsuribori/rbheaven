## RBHeaven

Site for discussing anything, anonymously.

## Setup

Django secret key and postgres password are read as Docker secrets from
`key.txt` and `password.txt`, respectively. Create these two files on the same
level as README.md and add your passwords to them.

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
