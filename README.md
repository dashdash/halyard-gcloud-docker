# Docker for Halyard and Google Cloud SDK

Docker image containing [Halyard](https://github.com/spinnaker/halyard) (tool for configuring and deploying [Spinnaker](https://www.spinnaker.io)) and the [Google Cloud SDK](https://cloud.google.com/sdk/).

## Usage

You can use it in the same way as the base Halyard image (see [here](https://www.spinnaker.io/setup/install/halyard/#install-halyard-on-docker)).  
Example:

```bash
docker run -p 8084:8084 -p 9000:9000 \
    --name halyard-gcloud --rm \
    -v ~/.hal:/home/spinnaker/.hal \
    -it \
    equalsmagic/halyard-gcloud:latest
```

## Tags

* `equalsmagic/halyard-gcloud:latest` - The latest available version
* `equalsmagic/halyard-gcloud:VERSION` - A specific halyard version
