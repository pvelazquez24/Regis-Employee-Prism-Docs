## Endpoint

``` bash
GET /clientMaster/getClientCodes
```
## Prism Fields
```csharp
public class PrismGetClientCodeDTO
{
    public ClientCodeDTO ClientCodes { get; set; }

    public class ClientCodeDTO
    {
        public int ClientId { get; set; }

        public List<ClientDepartmentDTO> DepartmentCode { get; set; }

        public class ClientDepartmentDTO
        {
            public int Id { get; set; }
            public string DeptName { get; set; }
        }

        public List<BenefitGroupCodeDTO> BenefitGroupCode { get; set; } = new List<BenefitGroupCodeDTO>();

        public class BenefitGroupCodeDTO
        {
            public int Id { get; set; }
            public string Description { get; set; }
        }
    }
}
```