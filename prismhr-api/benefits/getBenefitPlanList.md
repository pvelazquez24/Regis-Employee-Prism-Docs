## Endpoint

``` bash
GET /benefits/v1/getBenefitPlanList
```
## Prism Fields
```csharp
public class BenefitPlanListDTO
{
    public List<BenefitPlanItemDTO> BenefitPlanList { get; set; } = new List<BenefitPlanItemDTO>();
}

public class BenefitPlanItemDTO
{
    public string PlanId { get; set; }
    public string PlanDesc { get; set; }
    public string InsuranceClass { get; set; }
    public string InsuranceClassDesc { get; set; }
}
```