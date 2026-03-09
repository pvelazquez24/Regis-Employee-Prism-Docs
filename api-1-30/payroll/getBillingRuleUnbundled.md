## Endpoint

``` bash
GET /payroll/getBillingRuleUnbundled
```
## Prism Fields
```csharp
public class BillingRuleUnbundleDTO
{
    public BillingRuleUnbundleDetailDTO BillingRuleUnbundled { get; set; }

    public class BillingRuleUnbundleDetailDTO
    {
        public string BillingRuleNum { get; set; }
        public string Description { get; set; }
        public decimal Rate { get; set; }
        public string BasedOn { get; set; }
        public DateTime? StartDate { get; set; }
        public DateTime? EndDate { get; set; }
        public bool VoucherTypeRegular { get; set; }
        public bool VoucherTypeVacation { get; set; }
        public bool VoucherTypeSupplemental { get; set; }
        public bool VoucherTypeArrearage { get; set; }
        public bool VoucherTypeAdjustment { get; set; }
        public string EmployeeId { get; set; }
        public string Position { get; set; }
        public string BillingCode { get; set; }
        public string PayGroup { get; set; }
    }
}
```