## Endpoint

``` bash
GET /benefits/getClientBenefitPlanSetupDetails
```
## Prism Fields
```csharp
public class PrismBenefitPlanSetupDetailDTO
{
    public BenefitPlanDetailDTO BenefitPlanDetail { get; set; }

    public class BenefitPlanDetailDTO
    {
        public string PlanId { get; set; }
        public string TpaPlanIdOvr { get; set; }
    }
}
```