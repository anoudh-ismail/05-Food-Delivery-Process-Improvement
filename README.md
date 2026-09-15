# Food Delivery Order Fulfillment Process Improvement

## Business Analysis Case Study

**Case Study Organization:** Zomato  
**Industry:** Online Food Delivery  
**Project Type:** Business Process Improvement  
**Role:** Business Analyst — Portfolio Case Study  
**Case Study Basis:** Publicly available Zomato information

> **Disclaimer:** This is an independent portfolio case study based on publicly available information about Zomato's food-delivery operations. It does not represent an internal Zomato project and does not use confidential company data.

## Project Overview

This case study evaluates the food-delivery order fulfillment journey from order confirmation through final customer delivery. It focuses on operational bottlenecks, customer visibility, delivery coordination, exception handling, and SLA-based escalation.

**Workflow:** Industry evidence → Business problem → Stakeholders → As-Is process → Root-cause analysis → Gap analysis → To-Be process → Requirements → User stories → Acceptance criteria → UAT → Recommendations

## Business Objectives

The case study uses **assumed planning baselines and proposed targets** to demonstrate measurable process improvement.

| Objective | Assumed Baseline | Proposed Target |
|---|---:|---:|
| Late delivery rate | 18% | <5% |
| Delay-related support contacts | 100% baseline | -40% |
| Fulfillment cycle time | 100% baseline | -15% |
| Avoidable cancellations | 100% baseline | -25% |

> These values are portfolio-case assumptions, not verified internal Zomato performance figures.

## Stakeholders

Customers, Restaurants/Merchants, Delivery Partners, Customer Support, Operations, and Product/Technology teams.

## As-Is Process

Customer places order → Restaurant receives order → Restaurant accepts order → Food preparation → Delivery partner assigned → Rider travels to restaurant → Food picked up → Rider travels to customer → Customer receives order → Order completed.

Key pain points include preparation-time mismatch, dispatch/readiness coordination gaps, ETA inaccuracy when conditions change, and reactive delay communication.

## Root Cause & Gap Analysis

The major capability gaps identified are:

- **Visibility gap:** limited continuous visibility into preparation and delivery conditions.
- **Coordination gap:** restaurant readiness and delivery-partner dispatch need tighter synchronization.
- **Escalation gap:** operational teams need defined rules for identifying and escalating SLA breaches before problems become customer complaints.

## To-Be Process

Dynamic preparation-time estimation → Preparation monitoring → Optimized rider dispatch → Food-ready confirmation → Real-time tracking and dynamic ETA → Delay detection → Proactive notification / SLA escalation → Operations intervention → Successful delivery.

## Proposed SLA Rules

- **7 minutes:** If an order is not marked Ready within 7 minutes of estimated preparation time, alert Operations Dispatch.
- **10 minutes:** If predicted delivery delay exceeds 10 minutes, notify the customer with an updated ETA.
- **20 minutes:** If predicted delivery delay exceeds 20 minutes, escalate to Operations Support.

> These SLA thresholds are proposed case-study rules and are not claimed to be Zomato's internal thresholds.

## Requirements & Agile Artifacts

The project includes Business Requirements, Functional Requirements, requirements traceability, User Stories, Acceptance Criteria, UAT, and edge-case scenarios.

## Edge Cases Covered

- Rider accepts and then drops an order
- Restaurant repeatedly changes preparation time
- GPS signal is lost during active delivery
- Restaurant cancels after accepting an order
- Customer contacts support about a delayed order
- Delayed order is successfully recovered after intervention

## Recommendations

1. Introduce dynamic preparation-time monitoring.
2. Improve coordination between food readiness and rider dispatch.
3. Implement dynamic ETA recalculation.
4. Introduce proactive customer delay notifications.
5. Implement SLA-based operational escalation.
6. Standardize recovery for rider drop-offs and delivery exceptions.
7. Provide centralized operational visibility for Operations and Support.

## Expected Business Impact

The proposed process is intended to support improved delivery reliability, better customer transparency, faster operational intervention, lower delay-related support workload, lower avoidable cancellation risk, and improved fulfillment efficiency.

These outcomes should be validated with production performance data after implementation. This portfolio case study does not claim measured business results.

## Deliverables

### Documents
- `Documents/Food-Delivery-Order-Fulfillment-Process-Improvement-BA-Case-Study.docx`
- `Documents/Food-Delivery-Order-Fulfillment-Process-Improvement-BA-Case-Study.pdf`

### Process Maps
- `Process-Maps/As-Is-Process-Map.drawio`
- `Process-Maps/As-Is-Process-Map.png`
- `Process-Maps/To-Be-Process-Map.drawio`
- `Process-Maps/To-Be-Process-Map.png`

## BA Skills Demonstrated

Business problem definition, stakeholder analysis, process analysis, As-Is / To-Be mapping, root-cause and gap analysis, business and functional requirements, requirements traceability, user stories, acceptance criteria, SLA definition, UAT planning, edge-case analysis, KPI/target definition, and business recommendations.

## Industry References

1. **Zomato.** *The Deep Tech Behind Estimating Food Preparation Time.*  
   https://www.zomato.com/blog/food-preparation-time/

2. **Zomato Developer Platform.** *Restaurant Confirms Order on Zomato Logistics.*  
   https://www.zomato.com/developer/integration/docs/getting-started/development-for-integration/live-order-flow/restaurant-confirms-order/zomato-logistics/

> Public sources establish industry context and publicly documented process concepts. The proposed improvements, assumptions, requirements, SLAs, and UAT scenarios are original portfolio analysis.
