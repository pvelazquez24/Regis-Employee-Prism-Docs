## Endpoint

``` bash
GET /employee/getEmployee
```
## Prism Fields
```csharp
public class PrismClientGetEmployeeInformationDTO
{
    public int clientId { get; set; }
    public List<EmployeeDTO> Employee { get; set; } = new List<EmployeeDTO>();

    public class EmployeeDTO
    {
        public string RegisClientId { get; set; }
        public string Id { get; set; }
        public string FirstName { get; set; }
        public string LastName { get; set; }
        public string MiddleInitial { get; set; }
        public string BirthDate { get; set; }
        public string MobilePhone { get; set; }
        public string EmailAddress { get; set; }
        public string Gender { get; set; }
        public string MaritalStatus { get; set; }
        public string AddressLine1 { get; set; }
        public string AddressLine2 { get; set; }
        public string City { get; set; }
        public string State { get; set; }
        public string ZipCode { get; set; }
        public ClientDTO Client { get; set; }
        public string PeoStartDate { get; set; }
        public List<PlanDTO> Plan { get; set; } = new List<PlanDTO>();
        public string Subscriber { get; set; }
        public string DateGenerate { get; set; }
        public string Relation { get; set; }
        public string HomePhone { get; set; }
        public string maintenceTypeCode { get; set; }
        public CompensationDTO Compensation { get; set; }

        public class CompensationDTO
        {
            public string Ssn { get; set; }
            public string SsnUse { get; set; }
            public string CitizenshipStatus { get; set; }
        }

        public class ClientDTO
        {
            public string EmployeeStatus { get; set; }
            public string JobStartDate { get; set; }
            public string FirstHireDate { get; set; }
            public string LastHireDate { get; set; }
            public string StatusDate { get; set; }
            public string EmployeeType { get; set; }
            public string AddressLine1 { get; set; }
            public string AddressLine2 { get; set; }
            public string City { get; set; }
            public string State { get; set; }
            public string Zip { get; set; }
            public string WorkPhone { get; set; }
            public string EmailAddress { get; set; }
            public string PrimaryEmailSource { get; set; }
            public AssignmentDTO Assignment { get; set; }

        }

        public class AssignmentDTO
        {
            public string HomeLocation { get; set; }
        }

        public class PlanDTO
        {
            public string PlanId { get; set; }
            public string InsClass { get; set; }
            public string CoverageStart { get; set; }
            public string CoverageEnd { get; set; }
            public string Status { get; set; }
            public string CarrierPlanId { get; set; }
            public string CarrierEmployeeId { get; set; }
            public string EffectiveDate { get; set; }
            public string PlanType { get; set; }
            public string Polyce { get; set; }
            public string Custumer { get; set; }
            public string PlanIdSufix { get; set; }
            public List<DependentDTO> Dependent { get; set; } = new List<DependentDTO>();
            public class DependentDTO
            {
                public string DependentEmployeeId { get; set; }
                public string CoverageStart { get; set; }
                public string CoverageEnd { get; set; }
            }
        }
    }
}
```