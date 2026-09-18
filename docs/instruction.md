# Ingesting data

- Download the dataset from 'data/source/data.txt'
- create an EC2 instance > Docker container > "mcr.microsoft.com/mssql/server:2022-latest"
- Spin up legacy MySql server
```
docker run -e "ACCEPT_EULA=Y" -e "MSSQL_SA_PASSWORD=FdeProject@123" -p 1433:1433 --name mssql-container -d mcr.microsoft.com/mssql/server:2022-latest
```

- install the requirements 