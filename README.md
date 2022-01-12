# German-language periodicals published in Pilsen (CdV Ost³ 2022)

Selected German-language periodicals published in Pilsen covering the second half of the 19th century, reporting on local and supra-regional events. All metadata, text content (ALTO) and page images are available within the API.

The dataset includes following titles:

| Title                                                                                                  | UUID                                      |
| ------------------------------------------------------------------------------------------------------ | ----------------------------------------- |
| [Pilsner Anzeiger](https://kramerius.svkpk.cz/periodical/uuid:0561dab7-43c0-48e4-9a87-e1be12e67d3c)    | uuid:0561dab7-43c0-48e4-9a87-e1be12e67d3c |
| [Der Pilsner Bote](https://kramerius.svkpk.cz/periodical/uuid:deef7979-70d9-455d-85d8-0d762fedfd80)    | uuid:deef7979-70d9-455d-85d8-0d762fedfd80 |
| [Pilsner Reform](https://kramerius.svkpk.cz/periodical/uuid:f85d98aa-5bc0-4b2a-b105-4378fe8e22dd)      | uuid:f85d98aa-5bc0-4b2a-b105-4378fe8e22dd |
| [Pilsner Tagblatt](https://kramerius.svkpk.cz/periodical/uuid:300d84a7-4542-4767-8c76-dc7d708e1fba)    | uuid:300d84a7-4542-4767-8c76-dc7d708e1fba |
| [Pilsner Wochenblatt](https://kramerius.svkpk.cz/periodical/uuid:29fb39d3-ed76-4d32-ac2c-194227640f9f) | uuid:29fb39d3-ed76-4d32-ac2c-194227640f9f |
| [Pilsner Zeitung](https://kramerius.svkpk.cz/periodical/uuid:83190be2-3417-44a3-a501-55ccbcba5437)     | uuid:83190be2-3417-44a3-a501-55ccbcba5437 |


## API documentation
### Title level

Example for [Der Pilsner Bote](https://kramerius.svkpk.cz/periodical/uuid:deef7979-70d9-455d-85d8-0d762fedfd80) *uuid:deef7979-70d9-455d-85d8-0d762fedfd80*

**List of streams**

GET https://kramerius.svkpk.cz/search/api/client/v7.0/items/uuid:deef7979-70d9-455d-85d8-0d762fedfd80/info/data

**MODS**

GET https://kramerius.svkpk.cz/search/api/client/v7.0/items/uuid:deef7979-70d9-455d-85d8-0d762fedfd80/metadata/mods

**DC**

GET https://kramerius.svkpk.cz/search/api/client/v7.0/items/uuid:deef7979-70d9-455d-85d8-0d762fedfd80/metadata/dc

**List of child objects (volumes)**

GET https://kramerius.svkpk.cz/search/api/client/v7.0/search?q=own_parent.pid:%22uuid:deef7979-70d9-455d-85d8-0d762fedfd80%22

### Volume level

Example for [Der Pilsner Bote 13 (1869)](https://kramerius.svkpk.cz/periodical/uuid:6130f684-6e86-4d6a-a1df-96bfeb5959f1) *uuid:6130f684-6e86-4d6a-a1df-96bfeb5959f1*

**List of child objects (issues)**

GET https://kramerius.svkpk.cz/search/api/client/v7.0/search?q=own_parent.pid:%22uuid:6130f684-6e86-4d6a-a1df-96bfeb5959f1%22

### Issue level

Example for [Der Pilsner Bote 13(5) (17 January 1869)](https://kramerius.svkpk.cz/view/uuid:311de1df-994f-4e7e-8c67-cb50237f3104) *uuid:311de1df-994f-4e7e-8c67-cb50237f3104*

**List of child objects (pages)**

GET https://kramerius.svkpk.cz/search/api/client/v7.0/search?q=own_parent.pid:%22uuid:311de1df-994f-4e7e-8c67-cb50237f3104%22

### Page level

Example for [Der Pilsner Bote 13(5) (17 January 1869), p. 1](https://kramerius.svkpk.cz/view/uuid:9d903a75-4172-4bda-b0d3-a4bec2e719cc?page=uuid:766f9190-569d-11ec-bd75-001b63bd97ba) *uuid:d4b5dcac-50df-11ec-b6d4-001b63bd97ba*

**List of streams**

GET https://kramerius.svkpk.cz/search/api/client/v7.0/items/uuid:d4b5dcac-50df-11ec-b6d4-001b63bd97ba/info

**Full image**

GET https://kramerius.svkpk.cz/search/api/client/v7.0/items/uuid:d4b5dcac-50df-11ec-b6d4-001b63bd97ba/image

**ALTO (if exists)**

GET https://kramerius.svkpk.cz/search/api/client/v7.0/items/uuid:d4b5dcac-50df-11ec-b6d4-001b63bd97ba/ocr/alto

**Text (if exists)**

GET https://kramerius.svkpk.cz/search/api/client/v7.0/items/uuid:d4b5dcac-50df-11ec-b6d4-001b63bd97ba/ocr/text

### Other

**Item thumbnail or thumbnail of its child item**

GET https://kramerius.svkpk.cz/search/api/client/v7.0/items/uuid:d4b5dcac-50df-11ec-b6d4-001b63bd97ba/image/thumb
