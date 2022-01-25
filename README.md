# orgChart


graph LR
subgraph dir[Board of Directors]
a[John Smith]
b[Daniel Johnson]
c[Matthew Jones]
end

b-->ceo[CEO]

ceo-->coo[COO]
ceo-->cto[CTO]
ceo-->cfo[CFO]

coo-->vpmark[VP Marketing]
coo-->vphr[VP Human Resources]

subgraph Engineering
cto-->new[New Solutions Mgr]
cto-->old[Customer Support Mgr]
end

subgraph Finance
cfo-->recv[Acct Recv Mgr]
cfo-->payable[Acct Payable Mgr]
end

subgraph Sales and Marketing
vpmark-->sales[Sales Mgr]
vpmark-->mark[Marketing Mgr]
end

subgraph Human Resources
vphr-->hiring[Hiring Mgr]
vphr-->onboarding[Onboarding Mgr]
end

cto-.->contractor[Design Contractor]
cfo-.->accountant[Chartered Accountant]
