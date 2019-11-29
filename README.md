# nginx reverse proxy

## how to add your own uri

Fork this repository.

Clone this repository locally.

Get the private IP address of your instance.

Add another `location` block in the `server` block in the `nginx.conf` file in this repository:

```
location /MY_UNIQUE_NAME {
  proxy_pass http://PRIVATE_INSTANCE_IP_HERE/;
}
```

Commit & push these changes to your fork in github.

Open a pull request to this repository with your changes.

Ping us and we'll merge it! The changes should be automagically deployed and your environment should be internet-exposed very soon.
