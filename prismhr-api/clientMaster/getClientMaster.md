## Endpoint

``` bash
GET /clientMaster/v1/getClientMaster
```
## Prism Fields
```csharp
public class PrismPayrollClientMasterResultDTO
{
    public PrismPayrollClientMasterItemDTO ClientMaster { get; set; } = new PrismPayrollClientMasterItemDTO();
}
public class PrismPayrollClientMasterItemDTO
{
    public int ClientId { get; set; }
    public string ClientName { get; set; }
    public string Status { get; set; }
    public DateTime? StatusDate { get; set; }
    public string ServiceType { get; set; }
    public string StateCode { get; set; }
    public string ZipCode { get; set; }
    public int? EmployerId { get; set; }
    public string AddressLine1 { get; set; }
    public string AddressLine2 { get; set; }
    public string City { get; set; }
    public string Consultant { get; set; }
    public string Salesperson { get; set; }
    public string PayrollRep { get; set; }
    public string Broker { get; set; }
    public string RiskManager { get; set; }
    public string CostCenter { get; set; }
}

public class PrismPayrollClientListDTO
{
    public List<PrismPayrollClientListItem> ClientList { get; set; } = new List<PrismPayrollClientListItem>();
}

public class PrismPayrollClientListResultDTO
{
    public PrismPayrollClientListDTO ClientListResult { get; set; } = new PrismPayrollClientListDTO();
}
```