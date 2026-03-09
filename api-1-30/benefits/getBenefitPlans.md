## Endpoint

``` bash
GET /benefits/getBenefitPlans
```
## Prism Fields
```csharp
public class PrismBenefitBenefitPlanDTO
{
    public List<BenefitPlanDTO> BenefitPlan { get; set; } = new List<BenefitPlanDTO>();

    public class BenefitPlanDTO
    {
        public string PlanId { get; set; }
        public string InsClass { get; set; }
        public string CoverageStart { get; set; }
        public string CoverageEnd { get; set; }
        public string Status { get; set; }
        public string CarrierPlanId { get; set; }
        public string CarrierEmployeeId { get; set; }
        public List<PlanDetailDTO> PlanDetail { get; set; } = new List<PlanDetailDTO>();
        public class PlanDetailDTO
        {
            public string EffectiveDate { get; set; }
            public string PlanType { get; set; }
            public List<DependentDTO> Dependent { get; set; } = new List<DependentDTO>();
            public class DependentDTO
            {
                public string DependentId { get; set; }
                public string CoverageStart { get; set; }
                public string CoverageEnd { get; set; }
            }
        }
    }
}
```