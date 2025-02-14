# base build image

FROM mcr.microsoft.com/dotnet/sdk:8.0-jammy

# install azure articats credential provider (https://github.com/Microsoft/artifacts-credprovider)
RUN curl -sL https://raw.githubusercontent.com/Microsoft/artifacts-credprovider/master/helpers/installcredprovider.sh  | sh

# install nodejs 16 into the image
RUN curl -sL https://deb.nodesource.com/setup_16.x | bash
RUN apt-get install nodejs -y
RUN npm install --global yarn