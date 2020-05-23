Potential Ideas:

[Current UBI Week Which Will Be Incremental Every Sunday Night at 11:59PM]
[When UBIWeek Hits 17 Enable Set TaxCreditWeek to 1 & Pay Pool Tax Credit For Universal Basic Income Program]
UBIWeek = 1;
If(UBIWeek = Sunday) {
UBIWeek++;
If(UBIWeek = 17) {
TaxCreditWeek = 1;
IssueTaxCredit = True;
}

[Current TaxCreditWeek Which Will Be Incremental Every Sunday Night]
TaxCreditWeek = 0;

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

[Calculate TaxPool For Basic UBI]
BasicTaxPool = TaxPool - NodeRewards
[Calculate TaxPool For Node UBI][Users Who Run Nodes Get Double Tax Credit Rewards As Compared To Regular Users]
NodeTaxPool = (NodeRewards / ActiveNodeWallets)

[Reward Set Aside For Node Wallets]
TaxPoolNodeReward = (Taxpool * 2)

[Check Wallets Running Nodes]
ValidateWalletRunningNode();

[Amount Of Active Node Wallets]
TotalNodeWallets = ActiveNodeWallets


[Blockchain must record and add activeusers to a pool of wallets for future UBI payments]
[Blockchain must record payments of UBI to active users & node running users]
[UBICredit cannot double pay any 1 wallet more than is entitled]
