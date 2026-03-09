## Endpoint

``` bash
GET /generalLedger/getClientGLData
```
## Prism Fields
```csharp
public class PrismUrlDownloadDTO
{
    public string DownloadId { get; set; }
    public string BuildStatus { get; set; }
    public string DataObject { get; set; }
    public string ErrorCode { get; set; }
    public string ErrorMessage { get; set; }
}
```