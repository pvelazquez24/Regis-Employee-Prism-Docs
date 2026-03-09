## Endpoint

``` bash
GET /clientMaster/getClientMaster
```
## Prism Fields
```csharp
public class ClientMasterGetMasterDTO
{
    public ClientMasterDTO ClientMaster { get; set; }

    public class ClientMasterDTO
    {
        public int EmployerId { get; set; }
        public string CostCenter { get; set; }
    }
}
```