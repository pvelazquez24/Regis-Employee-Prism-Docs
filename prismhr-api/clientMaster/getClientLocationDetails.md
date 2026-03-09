## Endpoint

``` bash
GET /clientMaster/v1/getClientLocationDetails
```
## Prism Fields
```csharp
public class PrismGroupBenefitPlanDTO
{
    public PrismGroupBenefitPlanDetailDTO GroupBenefitPlan { get; set; }
}
public class PrismGroupBenefitPlanDetailDTO
{ 
    public string PlanId { get; set; }
    public string PlanDescription { get; set; }
    public string BillCode { get; set; }
}
```