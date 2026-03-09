## Endpoint

``` bash
GET /payroll/v1/getPayrollVouchers
```
## Prism Fields
```csharp
public class PrismPayrollVoucherForEmployeeDTO
{
    public List<PayrollVoucherDTO> PayrollVoucher { get; set; } = new List<PayrollVoucherDTO>();
}

public class PayrollVoucherDTO
{
    public string VoucherId { get; set; }
    public string BatchId { get; set; }
    public decimal? NetPay { get; set; }
    public string PayDate { get; set; }
    public string PayPeriodStart { get; set; }
    public string PayPeriodEnd { get; set; }
    public string EmployeeId { get; set; }
    public string CheckAccountACH { get; set; }
    public decimal? CheckAmt { get; set; }
    public decimal TotalEarnings { get; set; }
    public List<EarningDTO> Earning { get; set; } = new List<EarningDTO>();
    public List<EmployeeTaxDTO> EmployeeTax { get; set; } = new List<EmployeeTaxDTO>();
    public List<DeductionDTO> Deduction { get; set; } = new List<DeductionDTO>();
    public List<FromArrearsDTO> FromArrears { get; set; } = new List<FromArrearsDTO>();
    public List<OtherDeductionDTO> OtherDeduction { get; set; } = new List<OtherDeductionDTO>();
    public List<BenefitDTO> Benefit { get; set; } = new List<BenefitDTO>();
    public List<WorkerCompDTO> WorkerComp { get; set; } = new List<WorkerCompDTO>();
    public List<CompanyTaxDTO> CompanyTax { get; set; } = new List<CompanyTaxDTO>();
    public List<OtherEarningsDTO> OtherEarningsDetail { get; set; } = new List<OtherEarningsDTO>();
}

public class EarningDTO
{
    public string PayCode { get; set; }
    public string PayClass { get; set; }
    public string ProjWork { get; set; }
    public string Shift { get; set; }
    public decimal HoursUnits { get; set; }
    public decimal UnitRate { get; set; }
    public decimal PayAmount { get; set; }
}

public class EmployeeTaxDTO
{
    public string EmpTaxDeductCode { get; set; }
    public string EmpTaxDeductCodeDesc { get; set; }
    public decimal? EmpTaxableAmount { get; set; }
    public decimal? EmpTaxAmount { get; set; }
}

public class DeductionDTO
{
    public string DeductCode { get; set; }
    public string DeductDescription { get; set; }
    public string DeductType { get; set; }
    public decimal DeductAmount { get; set; }
}
public class FromArrearsDTO
{
    public string DedCode { get; set; }
    public string DedDescription { get; set; }
    public decimal ArrearsAmt { get; set; }
}
public class OtherDeductionDTO
{
    public string OtherDeductCode { get; set; }
    public string OtherDeductDescription { get; set; }
    public decimal OtherDeductAmount { get; set; }
}

public class BenefitDTO
{
    public string PlanId { get; set; }
    public decimal PremiumAmt { get; set; }
}

public class WorkerCompDTO
{
    public string WcClass { get; set; }
    public string WcTaxablePay { get; set; }
    public decimal WcBillAmount { get; set; }
    public decimal WcPremAmount { get; set; }
}

public class CompanyTaxDTO
{
    public string ComTaxDeductCode { get; set; }
    public string ComTaxDeductCodeDesc { get; set; }
    public decimal? ComTaxAmount { get; set; }
    public decimal? ComTaxableAmount { get; set; }
}

public class OtherEarningsDTO
{
    public string OtherEarnCode { get; set; }
    public string OtherEarnsDesc { get; set; }
    public decimal OtherEarnAmount { get; set; }
}

