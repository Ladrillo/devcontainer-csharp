FROM mcr.microsoft.com/devcontainers/dotnet:1-8.0-bookworm

# Update the package manager
RUN apt-get update -y

# Set the working directory
WORKDIR /workspaces

# Update workloads
RUN dotnet workload update

# Install dotnet-script globally
RUN dotnet tool install -g dotnet-script

# Add global tools to PATH
ENV PATH="${PATH}:/root/.dotnet/tools"

# Default command for debugging
CMD ["/usr/bin/zsh"]
