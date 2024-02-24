# SQL Server Docker container

How to pull and run the SQL Server Docker container 

We run Docker Desktop application

![image](https://github.com/luiscoco/Identity_dotNET8_Authentication/assets/32194879/be7cb784-9f18-4f5f-a557-cfcc47cc3d6f)

We open a command prompt window and run the following command

```
docker run ^
  -e "ACCEPT_EULA=Y" ^
  -e "MSSQL_SA_PASSWORD=Luiscoco123456" ^
  -p 1433:1433 ^
  -d mcr.microsoft.com/mssql/server:2022-latest
```

![image](https://github.com/luiscoco/Identity_dotNET8_Authentication/assets/32194879/5661f705-44eb-4537-855e-ed04279d002e)

We can also see the image in Docker Desktop

![image](https://github.com/luiscoco/Identity_dotNET8_Authentication/assets/32194879/399896b3-0c2b-4ec0-acfc-b83f10691e5d)

And also we can see the running container in Docker Desktop

![image](https://github.com/luiscoco/Identity_dotNET8_Authentication/assets/32194879/9a1b0c37-5bc0-4129-987c-60f77db91448)

We run SSMS SQL Server Management Studio and we connect to the SQL Server running docker container

![image](https://github.com/luiscoco/Identity_dotNET8_Authentication/assets/32194879/161280ed-c082-458b-b5d0-8474c050be70)

![image](https://github.com/luiscoco/Identity_dotNET8_Authentication/assets/32194879/f3b9ffd8-e3ea-4418-9e32-c63a90fa8df6)

![image](https://github.com/luiscoco/Identity_dotNET8_Authentication/assets/32194879/844b1d77-0a27-49f8-9e47-dfc3413f3af8)

In the password we input **Luiscoco123456**, the same password as we provide when we run the SQL Server docker container

Now we can create a new database "**DotNet8Authentication**" for this sample

```
CREATE DATABASE DotNet8Authentication
GO
```

![image](https://github.com/luiscoco/Identity_dotNET8_Authentication/assets/32194879/e8ea8450-da3b-47da-bc05-26cf8df3cf2f)

We select the **Refresh** option in the database

![image](https://github.com/luiscoco/Identity_dotNET8_Authentication/assets/32194879/169c0f98-cb8b-4479-9731-efc3002761a7)

Now we can see the new database in the Databases tree

![image](https://github.com/luiscoco/Identity_dotNET8_Authentication/assets/32194879/5b1d90b3-5fec-4ef6-a528-70eabb798f98)
