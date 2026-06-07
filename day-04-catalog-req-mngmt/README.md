# DAY 4: How Companies Ask for Stuff

Imagine Techasya has 10,000 employees.

One morning:

Employee: "I need a laptop."

Nobody panics because nothing is broken.

This is NOT an Incident.

This is a Request.

## The Golden Rule

Incident = Fix something

Request = Get something

Examples:

❌ VPN stopped working → Incident

✅ Need VPN access → Request

❌ Laptop dead → Incident

✅ Need a new laptop → Request

## Service Catalog

Think Amazon for employees.

Instead of buying headphones and books, employees order:

* Laptops
* Software
* Access
* ID Cards
* HR Services

Everything lives in the Service Catalog.

## The Three Heroes

### REQ

The big container.

Employee says:

"I need a laptop and VPN access."

ServiceNow creates:

REQ001

This is the master order.

### RITM

Each item gets its own record.

REQ001
├── Laptop
└── VPN

becomes

RITM001
RITM002

Because different teams may work on each item.

### TASK

Actual work.

Laptop team receives:

TASK:
Configure laptop

VPN team receives:

TASK:
Grant VPN access

This is where work happens.

## My Memory Trick

Amazon Order

REQ = Order

RITM = Product

TASK = Warehouse Work

## If an interviewer asks

"What happens when a user requests a laptop?"

Answer:

Catalog Item
↓
REQ
↓
RITM
↓
TASK
↓
Laptop Delivered

Done.