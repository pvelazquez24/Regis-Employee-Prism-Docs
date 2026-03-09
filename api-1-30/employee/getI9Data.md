## Endpoint

``` bash
GET /employee/getI9Data
```
## Prism Fields
```csharp
public class PrismClientGetEmployeeI9DataDTO
{
    public int ClientId { get; set; }
    public string EmployeeId { get; set; }
    public SectionOneDTO SectionOne { get; set; }
    public SectionTwoDTO SectionTwo { get; set; }

    public class SectionOneDTO
    {
        public CitizenStatusDTO CitizenStatus { get; set; }

        public class CitizenStatusDTO
        {
            public string AlienRegistrationNumberUscisNumber { get; set; }
        }
    }

    public class SectionTwoDTO
    {
        public List<IdentityDocumentDTO> IdentityDocument { get; set; }

        public EmploymentAuthorizationDocumentDTO EmploymentAuthorizationDocument { get; set; }

        public class IdentityDocumentDTO
        {
            public string DocumentTitle { get; set; }
            public string PhrIssuingAuthorityCode { get; set; }
            public string DocumentNumber { get; set; }
            public string ExpirationDate { get; set; }
        }

        public class EmploymentAuthorizationDocumentDTO
        {
            public string DocumentTitle { get; set; }
            public string PhrIssuingAuthorityCode { get; set; }
            public string DocumentNumber { get; set; }
            public string ExpirationDate { get; set; }
        }
    }
}
```