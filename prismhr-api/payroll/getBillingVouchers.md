## Endpoint

``` bash
GET /payroll/v1/getBillingVouchers
```
## Prism Fields
```csharp
public class PrismBillingVoucherDTO
{
    public List<BillingVoucherDTO> BillingVoucher { get; set; } = new List<BillingVoucherDTO>();
}
public class BillingVoucherDTO
{
    public string VoucherId { get; set; }
    public string BatchNumber { get; set; }
    public string PayDate { get; set; }
    public string EmployeeId { get; set; }
    public string Invoice { get; set; }
    public string Compensation { get; set; }
    public List<SumBillingDTO> SumBilling { get; set; } = new List<SumBillingDTO>();
}
public class SumBillingDTO
{
    public string BillCode { get; set; }
    public string BillCodeDescription { get; set; }
    public decimal? BillAmt { get; set; }
}
```