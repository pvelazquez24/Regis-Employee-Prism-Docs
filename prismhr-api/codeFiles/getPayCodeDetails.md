## Endpoint

``` bash
GET /codeFiles/v1/getPaycodeDetails
```
## Prism Fields
```csharp
public class ClientPayCodeDetailsDTO
{
    public PayCodeDetailDTO PayCode { get; set; }
}
public class PayCodeDetailDTO
{
    public string Id { get; set; }
    public string PayDescription { get; set; }
}
```