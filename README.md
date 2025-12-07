# personal
# Build multi-architecture images locally
./docker-buildx.sh --build-arg RELEASE=latest

# Build and push to registry
./docker-buildx.sh --push

# Build specific version
./docker-buildx.sh --release v1.0.0 --push

# Build for custom registry
./docker-buildx.sh --registry your-registry.com --namespace yourname --push
