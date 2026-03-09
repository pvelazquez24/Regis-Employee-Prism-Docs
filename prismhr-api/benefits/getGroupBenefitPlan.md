## Endpoint

``` bash
GET /benefits/v1/getGroupBenefitPlan
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