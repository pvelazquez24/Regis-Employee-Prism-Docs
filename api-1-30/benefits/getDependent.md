## Endpoint

``` bash
GET /benefits/getDependent
```
## Prism Fields
```csharp
public class PrismBenefitGetActiveDependentDTO
{
    public List<DependentDTO> Dependent { get; set; }
    public class DependentDTO
    {
        public string RegisClientId { get; set; }
        public string DependentId { get; set; }
        public string FirstName { get; set; }
        public string LastName { get; set; }
        public string MiddleInitial { get; set; }
        public string Gender { get; set; }
        public string Birthdate { get; set; }
        public string Ssn { get; set; }
        public string Relation { get; set; }
        public string Status { get; set; }
        public string Address { get; set; }
        public string AddressLine2 { get; set; }
        public string City { get; set; }
        public string State { get; set; }
        public string Zip { get; set; }

    }
}
```