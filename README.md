# Data studio connector
## Create Google Analytics funnel, based on Sequence Segment

Google Analytics Sequence Segment lets you build any user flow using: events, pageviews and other.
When you create sequential segment a->b->c->d, add-on splits it in 4 subsegments:
1. a
2. a->b
3. a->b->c
4. a->b->c->d

and make 4 google analytics API requests

## Instalation

1. Open [connector](https://datastudio.google.com/datasources/create?connectorId=AKfycbwQ9774vh93_eKAhy9Qf5Phrvm7AsoVeE7VPd23No98RmdvRfE7ndwPzh4Jh5mKRjrn) (*).
2. Click authorization.
3. Fill in configuration:
    1) Choose Sequence Segment, if you don't have one add [demo segment](https://analytics.google.com/analytics/web/template?uid=BYYcDsLZSpuZNqSO9XZ-NQ) (**).
    2) Add Google Analytics viewID (***).
    3) Add segments readible name. Each step in new line (optional).
    4) Connect datasource.



![](i/funnelAddonConfig.png)
### Funnel Visualisation

Use 'Funnel Step' as dimension to build a funnel.

![](i/funnel.png)

(*) Connector:
Lastest version 0.1.1
https://datastudio.google.com/datasources/create?connectorId=AKfycbz1tFF2IRLljAH-O3AgAIsJE8DkAJK__Ti_j8cqiVMWYc3_ENK8UBCX091bMTJ9Tl9v

Production version 0.1.1
https://datastudio.google.com/datasources/create?connectorId=AKfycbz1tFF2IRLljAH-O3AgAIsJE8DkAJK__Ti_j8cqiVMWYc3_ENK8UBCX091bMTJ9Tl9v

lastest dev
https://datastudio.google.com/datasources/create?connectorId=AKfycbz0-VVDChZL29rJSQfPmLNNf93CT1p36k0AnRwaDmw

(**) Demo Sequence Segment
https://analytics.google.com/analytics/web/template?uid=BYYcDsLZSpuZNqSO9XZ-NQ

(***) Find your Google Analytics viewID in "Google Analytics Account Explorer"
https://ga-dev-tools.appspot.com/account-explorer/
[//]: i/gaSequence.png
