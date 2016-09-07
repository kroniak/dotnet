FROM kroniak/dotnet:latest

# Install node-js and npm
RUN mkdir warmup \  
    && cd warmup \  
    && dotnet new -t web \
    && dotnet restore \  
    && cd .. \  
    && rm -rf warmup \
    && rm -rf /tmp/NuGetScratch