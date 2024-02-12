# Phone-company-analysis
Data analysis of profits from a phone company

The datasets belongs to a telecom / phone company that offers to its customers two prepaid rates: Surf and Ultimate. Dataset has information regarding 500 customers of 2018. The main goal is to determine which plan is more profitable. Also, I will perform the following hypothesis tests:
- Average profit of Surf plan and Ultimate plan.
- Average profit of NY-NJ area and Other areas.

The phone company rounds seconds to minutes and megabytes to gigabytes. Each individual call is rounded, even if the call lasts 1 second, it will be charged and counted as 1 minute. Regarding internet, individual consumption will not be rounded, however the total amount rounds up. If anybody consumes 1025 megabytes then 2 gigabytes will be charged (1 GB = 1024 megabytes)

**Description of the plan rates:**

_Surf_

- Monthly payment: 20$
- 500 minutes, 50 SMS and 15 GB of data per month.

If these limits are exceeded, then:

- 1 extra minute: 3 cents
- 1 extra SMS: 3 cents
- 1 extra GB of data: 10$

_Ultimate_

- Monthly paymentl: 70$
- 3000 minutes, 50 SMS y 15 GB of data per month.

If these limits are exceeded, then:

- 1 extra minute: 1 cents
- 1 extra SMS: 1 cents
- 1 extra GB of data: 7 $

**Datasets:**

_users:_

- user_id — user's id
- first_name —user's name
- last_name — user's last name
- age — user's age (years)
- reg_date — registered date (dd, mm, aa)
- churn_date — date when user left the plan (if is a null value, it means the plan was being used in that date)
- city — user's city of residency
- plan — rate name

_calls:_

- id — call id
- call_date — call date
- duration — call duration (minutes)
- user_id — user's id

_messages:_

- id — sms id
- message_date — sms date
- user_id — user's id

_internet:_

- id — session id
- mb_used — data amount used in session (megabytes)
- session_date — session date
- user_id — user's id

_plans:_

- plan_name — rate name
- usd_monthly_fee — plan's monthly fee, expressed in united states dollars
- minutes_included — minutes included in the plan
- messages_included — SMS included in the plan
- mb_per_month_included — data included in the plan (megabytes)
- usd_per_minute — extra minute fee
- usd_per_message — extra sms fee
- usd_per_gb — extra gb fee
