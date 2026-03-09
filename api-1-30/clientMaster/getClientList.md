## Endpoint

``` bash
GET /clientMaster/getClientList
```
## Prism Fields
```csharp
public class PrismClientInformationDTO
{
    public ClientDTO ClientListResult { get; set; }

    public class ClientDTO
    {
        public List<ClientDetailDTO> ClientList { get; set; } = new List<ClientDetailDTO>();

        public class ClientDetailDTO
        {
            public int ClientId { get; set; }
            public string ClientName { get; set; }
            public string LegalName { get; set; }
            public string Status { get; set; }
        }
    }
}
```