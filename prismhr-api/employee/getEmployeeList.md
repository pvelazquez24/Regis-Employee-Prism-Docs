## Endpoint

``` bash
GET /employee/v1/getEmployeeList
```
## Prism Fields
```csharp
public class PrismClientEmployeeIdDTO
{
    public int ClientId { get; set; }
    public EmployeeNewDTO EmployeeList { get; set; }

    public class EmployeeNewDTO
    {
        public List<string> EmployeeId { get; set; } = new List<string>();
    }
}
```