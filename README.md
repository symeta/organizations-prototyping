# organizations-prototyping

## Pain Points Overview
Scaled customer who has multiple lines of business (LOB), especially business cross regions, or multiple system environments, e.g. UAT, SIT, Dev, Pre-Prod, Prod etc. always has multiple aws accounts to host these workloads, for easy of use, as well as to minimize the blase radius. However, this muti-account structure makes it difficult to operate and maintain unifiably. Plus, this kind of account structure makes billing & payment job much more complicated. 

Another issue the multi-account structure causes is that the legacy provisioned direct connection between an aws account and IDC cannot be shared with other accounts. 

Aws Organizations together with Single-Sign-On (SSO for short) provides a perfect solution to make it possible to achieve single sign on of different accounts under the umbrella account, as well as to achieve a consolidated billing and payment of all the accounts (Pls notice: after Organizations is initiated, the single account level billing could also be viewed by logining to that account, but cannot be paid through that account, could be paid through the umbrella account only).

Moreover, the Direct Connect instance could be shared between different accounts by associating the direct connect gateway to the virtual private gateways of other accounts.

## Table of Contents
- [1. Architecture Design](https://github.com/symeta/organizations-prototyping/tree/Architecture-Design)
- [2. Organizations Initialization](https://github.com/symeta/organizations-prototyping/tree/organization-initialization)
- [3. SSO Initialization]()
- [4. SSO to multi-accounts show case]()
- [5. Consolidated Billing & Account Level Billing show case]()
- [6. Direct Connect Gateway Sharing Configuration]()
