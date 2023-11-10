# Country-Service

![image](https://github.com/GalievDev/country-service/assets/96568075/45433bfd-0df6-4db4-b0e4-4ff3768da7f5)

### Task

Implement a microservice which provides a list of countries and, in addition, provides more detailed information per
country.

1. Use spring-boot
2. Use best practices and microservice approach
3. Implement the following REST API with spring-boot:

<details>
  <summary>GET /countries/</summary>

```json
{
  "countries": [
    {
      "name": "Finland",
      "country_code": "FI"
    }
  ]
}
```

</details>

<details>
  <summary>GET /countries/{name}</summary>

```json
{
  "name": "Finland",
  "country_code": "FI",
  "capital": "Helsinki",
  "population": 5491817,
  "flag_file_url": "<url to the flag file>"
}
```

</details>

5. Country service must fetch the relevant information for countries from some other service
    - You could use for example the following service: https://countriesnow.space/
6. Test the implementation as well as it's needed from your perspective
7. All the implementations must be runnable locally with our own computer. Write needed instructions to README.md file.
8. Publish all sources code and relevant files in github or similar service and send the link to the repo so that the
   implementation can be reviewed.

- You get bonus points if:
    - you use and understand reactor (https://www.baeldung.com/reactor-core)
    - you create a separate wep application which utilizes the created REST API and shows the relevant country
      information in a browser
