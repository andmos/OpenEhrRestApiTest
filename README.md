# OpenEHR REST API TEST
Test utility to verify the correctness of different OpenEhr REST API
implementations. See the 
[OpenEhr specification]( https://www.openehr.org/programs/specification/workingbaseline)
for more information.

Could be used as a .NET test project in existing implementations by adding it
as a git submodule.

# Run tests

```
    $ dotnet test
```

# Configuration 
It's possible to target differet OpenEHR REST API servers by modifying the
[settings.json](OpenEhrRestApiTest/settings.json) file:

```
{
    "ServerHostname": "localhost",
    "ServerPort":  "9000",
    "Protocol": "http"
}
```

# Test Data
Tests that require input data, such as creating a new composition, use test
data in [TestData](OpenEhrRestApiTest/TestData). These datasets should be
identical to the test data in the REST API Swagger docs.