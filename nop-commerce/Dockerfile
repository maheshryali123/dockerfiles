FROM mcr.microsoft.com/dotnet/aspnet:6.0
RUN mkdir -p /var/www/nopCommerce
RUN apt update
RUN apt install unzip wget -y
WORKDIR /var/www/nopCommerce
RUN wget https://github.com/nopSolutions/nopCommerce/releases/download/release-4.60.2/nopCommerce_4.60.2_NoSource_linux_x64.zip
RUN unzip nopCommerce_4.60.2_NoSource_linux_x64.zip
EXPOSE 80
CMD [ "dotnet", "Nop.Web.dll" ]