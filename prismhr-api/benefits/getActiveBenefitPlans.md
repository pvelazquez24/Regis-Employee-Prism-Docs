## Endpoint

``` bash
GET /benefits/v1/getActiveBenefitPlans
```
## Prism Fields
```csharp
public class PrismGetActiveBenefitPlanDTO
{
    public List<benefitPlanDTO> benefitPlan { get; set; } = new List<benefitPlanDTO>();
    public class benefitPlanDTO
    {
        public string planId { get; set; }
        public string description { get; set; }
        public string status { get; set; }
        public string insClass { get; set; }
        public List<planDetailDTO> planDetail { get; set; } = new List<planDetailDTO>();

        public class planDetailDTO
        {
            public string planType { get; set; }
        }
    }
}
```