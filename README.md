# Hostile

Create a hostile environment, perhaps a kubernetes cluster, where you can
stress-test your deployment. Verify things like security settings, do load
testing, restart pods often, etc.

## Input

- openapi (optional)
- deployment
- service

## Stuff to do

- docker inspect an image or a running container if possible,
  `docker inspect <image-name>`
- Check that the deployment has a good security context set
- Call all endpoints with weird stuff
- slowloris
- Restart pods often
- Have a stressed client deployment that gets angry if it can't access the
  service
