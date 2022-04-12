# Custom Ruby Versions for LTV

## Build Notes

### Multi Arch Build Example

    docker buildx create --use
    # omit the --push below if you do not have docker push access
    docker buildx build --platform linux/amd64,linux/arm64 --push -t beenverifiedinc/ruby:2.6.9-bullseye-slim-jemalloc .
