Potential Ideas:

[Current Tax Week Which Will Be Incremental Every Sunday Night]
TaxCreditWeek = 1;

[Current Status Of Tax Payments From Pool]
Boolean TaxCreditPaid = false;



[Set Tax For Transactions] 
Tax = 1%

[Set This Boolean To True To Issue Tax Credits From Pool But Must Return False After Credit's Are Paid]
IssueTaxCredit = True;

[Tax Credit Will Only Be Paid After Weekly Founder Rewards Are Paid]
While(TaxCreditWeek != 17){
IssueTaxCredit = false;
}

[Essentially Every Time
If(TaxCreditWeek = 18){
IssueTaxCredit = True;

[Total Tax Collected From Transactional Tax]
TaxPool = TransactionalTaxCollected

[Reward Set Aside For Node Wallets]
TaxPoolNodeReward = (Taxpool * 2)

[Amount Of Active Node Wallets]
TotalNodeWallets = ActiveNodeWallets

NodeReward = TaxCollected/ActiveNodeWallets

If(Running_Node) {
Tax
